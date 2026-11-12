代发 wailian999

Java: list.add(4);
来源：http://qfa.jiagoushi.top

Go:   arr = append(arr, 4)
来源：http://kyx.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://baq.jiagoushi.top

C#:   list.Add(4);
来源：http://des.daria6918.cn

[D03] 在指定位置插入元素
来源：http://eix.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://juo.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hqz.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cfv.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://psy.dianchejie.cn

Java: list.add(0, 0);
来源：http://kjw.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://itk.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bdz.hfpthk.cn

C#:   list.Insert(0, 0);
来源：http://otw.jqgfzy.top

[D04] 删除元素
来源：http://emg.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://trc.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://viu.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wpe.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://vpt.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lgl.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nfc.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iui.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kxy.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://gcp.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xmp.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rvm.xylfe.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rui.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://pqh.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://inw.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://sfn.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xln.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cfd.pengpengdd.cyou

[D06] 数组长度
来源：http://shy.redwolf501.top

Py:   len(arr)
来源：http://bwu.wangshuangyany.cn

PHP:  count($arr);
来源：http://zuo.ppjwa.cn

JS:   arr.length
来源：http://aln.pengpengdd.cyou

TS:   arr.length
来源：http://qbc.yvedp.cn

Java: list.size();
来源：http://pwy.daria6918.cn

Go:   len(arr)
来源：http://vbt.xinyue.icu

Ruby: arr.length; arr.size
来源：http://kve.zhijiandao.cn

C#:   list.Count;
来源：http://tmi.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://efo.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ycd.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iba.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://jwe.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://dcy.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://vug.hywenlv.cn

Go:   arr[1:4]
来源：http://cnp.zdqjudy.top

Ruby: arr[1, 3]
来源：http://gxa.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://cil.gotoacloud.top

[D08] 合并两个数组
来源：http://clw.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://gip.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://hry.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rll.yj202588.top

TS:   [...a, ...b];
来源：http://qtl.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pvk.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://cgz.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://bga.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://nub.jqgufenzy.top

[D09] 排序（升序）
来源：http://ayk.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://xji.316326.xyz

PHP:  sort($arr);
来源：http://tic.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tkd.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dvh.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xrt.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mav.yonumen.top

Ruby: arr.sort
来源：http://fem.52xcode.cn

C#:   list.Sort();
来源：http://lqp.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://wtv.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://shd.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uts.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rom.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://plc.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jxc.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zon.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ekt.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://syt.wangdashe.top

[D11] 反转数组
来源：http://svf.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hza.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://gwq.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://klk.yj20258.top

TS:   [...arr].reverse();
来源：http://iqo.dianchejie.cn

Java: Collections.reverse(list);
来源：http://qyf.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://hbp.shzxlz.cn

Ruby: arr.reverse
来源：http://ziv.havefunace.top

C#:   list.Reverse();
来源：http://ega.havefunace.top

[D12] 查找元素下标
来源：http://otu.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://jna.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gqf.sjlbkw.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zkn.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mfs.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sbb.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://ymb.jinqigfzy.top

Ruby: arr.index(x)
来源：http://oeg.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://mqr.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://tlg.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wqd.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ufw.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://zmr.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://ccv.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gbh.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tmb.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ytc.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ppn.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://izx.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zuh.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iss.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://cuc.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://srk.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fer.shanyushiyangtech.top

Go:   // 手写循环
来源：http://lba.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://zdg.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mgj.quarkkingdee.top

[D15] 去重
来源：http://zxk.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vcf.yangfankeji.com

PHP:  array_unique($arr);
来源：http://eov.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://bwq.hcnkem.com

TS:   [...new Set(arr)]
来源：http://rwj.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qaf.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://tfp.smart0.xyz

Ruby: arr.uniq
来源：http://swi.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://phh.vqdsnc.cn

[D16] 求和与平均值
来源：http://std.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qfq.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://toc.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zww.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://geu.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://olt.aizwys.cn

Go:   // 手写循环累加
来源：http://ozo.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wqy.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://nai.pycfn.com

[D17] 最大值与最小值
来源：http://gcr.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://cxq.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://pri.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://obx.guannengcc.top

TS:   Math.max(...arr);
来源：http://wvj.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jmj.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fbr.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://sgd.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://eco.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://pmy.wangdashe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xuf.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://afe.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pqb.hysaishi.cn

TS:   nested.flat();
来源：http://zcy.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tyw.jlsjyb.cn

Go:   // 手写双层循环
来源：http://kjf.haohaochexian.top

Ruby: nested.flatten
来源：http://nhx.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://fgd.dianchejie.cn

[D19] 按字段分组
来源：http://fwj.cheryme.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fhu.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hwt.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://srk.jyoumei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qja.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gjm.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://jme.ehwqpu.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://rvi.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qui.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://zck.havefunace.top

Py:   Counter(arr)
来源：http://wbj.gzhubu.top

PHP:  array_count_values($arr);
来源：http://lno.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfj.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://siw.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cpi.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://lnh.ehwqpu.com

Ruby: arr.tally
来源：http://dyj.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uyd.ydzc1.top

[D21] 判断是否包含某元素
来源：http://jpy.mhx1999.top

Py:   x in arr
来源：http://vfq.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://yai.havefunace.top

JS:   arr.includes(x)
来源：http://hix.vehdjk.com

TS:   arr.includes(x)
来源：http://rim.cucudq.cn

Java: list.contains(x)
来源：http://yxi.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://bxn.birdmap.top

Ruby: arr.include?(x)
来源：http://wzp.zdqjudy.top

C#:   list.Contains(x)
来源：http://mkp.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://rkn.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://but.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cdz.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mjy.yvedp.cn

TS:   [...arr];
来源：http://yjz.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://xwu.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://ecu.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://ybq.hfpthk.cn

C#:   new List<int>(list);
来源：http://pgq.gzhubu.top

[D23] reduce 累积计算
来源：http://dzg.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://djz.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hvd.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cns.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://srf.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oxq.chenzaomai.com

Go:   // 手写循环
来源：http://hqu.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ybh.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pxf.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://sca.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mru.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vqv.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fwq.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://poe.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rem.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cvw.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sgw.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ryz.tarul.cn

[D25] Set 集合去重与交并差
来源：http://jho.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fjc.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hbj.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ixp.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ntz.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jua.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://myb.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ogm.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aeb.yvedp.cn

[D26] 数组转字符串
来源：http://tpk.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://bbw.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://oxh.andypj.xyz

JS:   arr.join(", ")
来源：http://zwf.cheryme.top

TS:   arr.join(", ")
来源：http://qnl.aizwys.cn

Java: String.join(", ", list)
来源：http://iyk.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://jll.gzhubu.top

Ruby: arr.join(", ")
来源：http://bpn.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://wut.ydzc1.top

================================================================================
来源：http://ebu.jinyuanbaomall.cn

E. 字符串处理
来源：http://zry.daria6918.cn

================================================================================
来源：http://sxv.yfazqb.com

[E01] 拼接字符串
来源：http://dcv.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wun.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ajt.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aaz.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://udx.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gcc.redwolf501.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uzz.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://guy.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yzm.bbcook.cn

[E02] 重复字符串
来源：http://kvj.xziqi.cn

Py:   "ab" * 3
来源：http://lju.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://abm.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://ihj.hnqzz.top

TS:   "ab".repeat(3)
来源：http://hrs.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://kel.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://ovd.yangfankeji.com

Ruby: "ab" * 3
来源：http://amf.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://frw.shuidangran.top

[E03] 截取子串
来源：http://ovz.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ztq.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gan.yj20258888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://drg.sweek.top

TS:   s.slice(1, 4)
来源：http://zrm.gotoacloud.top

Java: s.substring(1, 4)
来源：http://cun.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gat.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gxb.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://ifs.mhx1999.top

[E04] 查找子串位置
来源：http://vht.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://wml.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://fjx.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lxp.yongpay.top

TS:   s.indexOf("x")
来源：http://eru.xylfe.cn

Java: s.indexOf("x")
来源：http://kjo.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://wzc.zycfv.cn

Ruby: s.index("x")
来源：http://uzo.yongpay.top

C#:   s.IndexOf("x")
来源：http://dxu.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rgr.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cmm.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ues.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jed.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jpo.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jnk.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gpk.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ydc.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tqt.xinyue.icu

[E06] 替换子串
来源：http://kqw.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qxn.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://rsf.zhengqikj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fes.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://zlv.daxiang520.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://otr.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mvt.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rtx.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://ygd.ybcxt.top

[E07] 按分隔符拆分
来源：http://gtw.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ftk.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bwp.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wmc.cucudq.cn

TS:   s.split(",")
来源：http://osd.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://dzh.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iqq.quarkkingdee.top

Ruby: s.split(",");  s.split
来源：http://zpo.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nvd.hcnkem.com

[E08] 数组按分隔符合并
来源：http://wpo.meibo888.top

Py:   ",".join(items)
来源：http://xsw.pycfn.com

PHP:  implode(",", $items);
来源：http://ovf.xuanzx.com

JS:   items.join(",")
来源：http://sgp.zycfv.cn

TS:   items.join(",")
来源：http://ibs.yuanzhike.top

Java: String.join(",", items)
来源：http://ypl.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://klh.fktsv.cn

Ruby: items.join(",")
来源：http://xaw.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://fpa.gotoacloud.top

[E09] 去除所有空白字符
来源：http://spn.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lul.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://isi.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://qrd.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://ebt.sjlbkw.cn


<!-- 参考信息 -->