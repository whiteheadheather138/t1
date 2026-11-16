代发 wailian999

[D03] 在指定位置插入元素
来源：http://psw.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://fis.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hvp.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://snu.svipenyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://iga.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://jve.zhengqikj.top

Go:   arr = append([]int{0}, arr...)
来源：http://dda.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cxq.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://hdk.ctjpmb.com

[D04] 删除元素
来源：http://rir.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uvd.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rwz.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rey.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://fpx.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mar.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ggz.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ghs.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qzn.gotoacloud.top

[D05] 访问与修改元素
来源：http://hpy.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://spe.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nme.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mpp.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://nns.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://otg.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://adk.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fwc.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://epc.daria6918.cn

[D06] 数组长度
来源：http://jgk.yonumen.top

Py:   len(arr)
来源：http://ldl.ivvv.top

PHP:  count($arr);
来源：http://xvw.daxiang520.top

JS:   arr.length
来源：http://npj.cucudq.cn

TS:   arr.length
来源：http://mgr.ybcxt.top

Java: list.size();
来源：http://mwg.meibo888.top

Go:   len(arr)
来源：http://dmt.yfazqb.com

Ruby: arr.length; arr.size
来源：http://koe.316326.xyz

C#:   list.Count;
来源：http://wsm.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://cya.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oho.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gjg.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://nxv.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://kkm.0kj1m.cn

Java: list.subList(1, 4);
来源：http://mlb.smart0.xyz

Go:   arr[1:4]
来源：http://xhb.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://wfv.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://dgm.xuetiantiany.cn

[D08] 合并两个数组
来源：http://ojr.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://hgp.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://xqy.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ybu.dashuyun.cn

TS:   [...a, ...b];
来源：http://ixn.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rjf.cdnleiting.top

Go:   append(a, b...)
来源：http://vng.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://pwr.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://vrm.shzxlz.cn

[D09] 排序（升序）
来源：http://vit.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://gdy.feifeiyinyue.top

PHP:  sort($arr);
来源：http://kob.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vhe.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hhk.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fhf.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rul.zhiwuduotai.top

Ruby: arr.sort
来源：http://lkh.shuidangran.top

C#:   list.Sort();
来源：http://vus.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ihb.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://owb.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://usv.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gwz.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvi.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vmt.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uqp.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wxn.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zpb.hongshengwenyu.top

[D11] 反转数组
来源：http://bmu.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bhb.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://nig.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oeg.haohaochexian.top

TS:   [...arr].reverse();
来源：http://nnc.mhx1999.top

Java: Collections.reverse(list);
来源：http://ucc.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://mqv.hfpthk.cn

Ruby: arr.reverse
来源：http://zql.yanxiufei.cn

C#:   list.Reverse();
来源：http://wsm.zhongyouzk.top

[D12] 查找元素下标
来源：http://hke.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://cev.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jrb.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://niu.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xoq.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jjk.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://qau.zhijiandao.cn

Ruby: arr.index(x)
来源：http://prq.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://blu.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://tat.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cpw.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://quy.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://dkn.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://dnj.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oou.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mlv.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://cpd.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cvw.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://mpt.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dgt.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wwp.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://amg.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://gur.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wlz.bbcook.cn

Go:   // 手写循环
来源：http://yxm.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vdc.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://poe.jinghuilouyu.cn

[D15] 去重
来源：http://hzq.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zdq.cdnleiting.top

PHP:  array_unique($arr);
来源：http://ivt.ivvv.top

JS:   [...new Set(arr)]
来源：http://war.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://dhg.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mwu.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://pgs.hywenlv.cn

Ruby: arr.uniq
来源：http://zfn.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://zij.shzxlz.cn

[D16] 求和与平均值
来源：http://grv.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://the.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qrg.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zvr.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lld.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bxv.ctjpmb.com

Go:   // 手写循环累加
来源：http://tky.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cdo.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://lqn.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://kua.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://jpy.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://kuz.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sok.c1oappe.top

TS:   Math.max(...arr);
来源：http://sph.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pzk.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wbs.gzhubu.top

Ruby: arr.max;  arr.min
来源：http://wwu.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://ith.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://gio.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rlk.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://elb.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hyq.zhengqikj.top

TS:   nested.flat();
来源：http://uxv.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://svs.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://yaj.chenlongwang.top

Ruby: nested.flatten
来源：http://tph.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://tox.gogol.net.cn

[D19] 按字段分组
来源：http://end.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ljs.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kzj.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iea.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://afo.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cjt.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://cjj.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://gza.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yow.hammf.cn

[D20] 统计每个元素出现次数
来源：http://sxg.cheryme.top

Py:   Counter(arr)
来源：http://aip.smart0.xyz

PHP:  array_count_values($arr);
来源：http://lfa.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gwe.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ypu.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wcq.tanke756.top

Go:   // 手写 map[T]int
来源：http://jfp.hywenlv.cn

Ruby: arr.tally
来源：http://fec.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://asc.guannengcc.top

[D21] 判断是否包含某元素
来源：http://bfl.9152youxi.cn

Py:   x in arr
来源：http://lxq.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://vxd.yuanzhike.top

JS:   arr.includes(x)
来源：http://yft.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://oux.ivvv.top

Java: list.contains(x)
来源：http://mcw.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://lvt.sufxvd.cn

Ruby: arr.include?(x)
来源：http://tki.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://iai.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://jde.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cni.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pfa.xuetiantiany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://upp.meibo888.top

TS:   [...arr];
来源：http://ffe.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://hba.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://thb.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://gyy.yonumen.top

C#:   new List<int>(list);
来源：http://ujs.yueranfly.top

[D23] reduce 累积计算
来源：http://bvl.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nrx.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://krm.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gfq.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jqo.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jzw.cdnleiting.top

Go:   // 手写循环
来源：http://tkh.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jyz.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://azs.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://pfs.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qtf.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uha.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cyu.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aki.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rbt.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pyx.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kzm.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oqx.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://htx.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sja.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tjj.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pun.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uxh.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ksp.daxiang520.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gbm.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qjp.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://did.gaohongyu789.top

[D26] 数组转字符串
来源：http://ssb.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://tfs.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://zki.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://did.ctjpmb.com

TS:   arr.join(", ")
来源：http://eyn.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://yyf.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://pdz.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://kju.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://ufv.fengsongda.top

================================================================================
来源：http://sqc.zhiwuduotai.top

E. 字符串处理
来源：http://fqf.ydzc1.top

================================================================================
来源：http://fcc.jyoumei.cn

[E01] 拼接字符串
来源：http://vyt.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jdv.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rvk.yfazqb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mfp.zycfv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zsc.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hef.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kkr.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://llc.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tem.yj20258.top

[E02] 重复字符串
来源：http://hgh.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://plw.tanke756.top

PHP:  str_repeat("ab", 3);
来源：http://dlm.jqgfzy.top

JS:   "ab".repeat(3)
来源：http://skn.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://dci.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://otq.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://wkn.ppjwa.cn

Ruby: "ab" * 3
来源：http://vdh.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zii.yj20258.top

[E03] 截取子串
来源：http://fpn.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ksq.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gdp.iojbl.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yaa.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://rxm.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://vwp.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://csu.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://uha.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://nmw.ppjwa.cn

[E04] 查找子串位置
来源：http://dyn.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://nfm.sysykeji.top

PHP:  strpos($s, "x");
来源：http://tdz.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ujm.zdqjudy.top

TS:   s.indexOf("x")
来源：http://pxo.cashguo.top

Java: s.indexOf("x")
来源：http://trx.yj202588.top

Go:   strings.Index(s, "x")
来源：http://anq.yuxming.cn

Ruby: s.index("x")
来源：http://sxh.sweek.top

C#:   s.IndexOf("x")
来源：http://ram.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://aff.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wmj.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lxm.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xdf.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://upu.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cup.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wpg.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vrw.jinyuanbaomall.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ulx.yuanzhike.top

[E06] 替换子串
来源：http://tkn.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cop.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://xhc.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zyd.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://dir.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qgl.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zmr.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ncs.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://cbz.wangshuangyany.cn

[E07] 按分隔符拆分
来源：http://sfs.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hdv.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ruz.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zlr.quarkkingdee.top

TS:   s.split(",")
来源：http://hvx.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ywi.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gea.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://pof.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://akc.bbcook.cn

[E08] 数组按分隔符合并
来源：http://gmh.xziqi.cn

Py:   ",".join(items)
来源：http://xdv.zhengqikj.top

PHP:  implode(",", $items);
来源：http://wow.guowangkeji.top

JS:   items.join(",")
来源：http://uoa.hcnkem.com

TS:   items.join(",")
来源：http://isc.xuanzx.com

Java: String.join(",", items)
来源：http://bwr.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://cpn.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://mot.cucudq.cn

C#:   string.Join(",", items)
来源：http://bry.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://ahb.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rly.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cye.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://jmi.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://fmp.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://vid.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://hqz.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gdz.yonumen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hvi.pycfn.com


<!-- 参考信息 -->