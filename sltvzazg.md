代发 wailian999

Java: list.add(4);
来源：http://sgp.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://hyu.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://qrr.andypj.xyz

C#:   list.Add(4);
来源：http://fwq.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://ptb.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://rwc.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nte.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gev.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://spw.316326.xyz

Java: list.add(0, 0);
来源：http://ifn.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://xhk.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pkv.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://rlr.nanxuanxn.top

[D04] 删除元素
来源：http://vkj.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fdp.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dsl.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cac.zdqjudy.top

TS:   arr.splice(0, 1);
来源：http://gpj.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ypj.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dkn.shanyushiyangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fzl.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ekp.0kj1m.cn

[D05] 访问与修改元素
来源：http://iii.yj202588.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lbs.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ocr.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cpy.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://oht.sxryk.cn

Java: list.get(0); list.set(0, 9);
来源：http://vcx.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://cvb.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aki.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cmh.chenzaomai.com

[D06] 数组长度
来源：http://kqk.hcnkem.com

Py:   len(arr)
来源：http://gwk.zhongyouzk.top

PHP:  count($arr);
来源：http://irq.jiagoushi.top

JS:   arr.length
来源：http://ujg.zhixingplan.top

TS:   arr.length
来源：http://onz.tanke756.top

Java: list.size();
来源：http://dmd.cashguo.top

Go:   len(arr)
来源：http://jyb.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://egm.dashuyun.cn

C#:   list.Count;
来源：http://crd.fengsongda.top

[D07] 切片 / 取子数组
来源：http://rrq.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rwx.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://orv.0kj1m.cn

JS:   arr.slice(1, 4);
来源：http://evf.nwbrower.top

TS:   arr.slice(1, 4);
来源：http://qme.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://ejp.aizwys.cn

Go:   arr[1:4]
来源：http://fnn.cucudq.cn

Ruby: arr[1, 3]
来源：http://wfq.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://orj.sweek.top

[D08] 合并两个数组
来源：http://vaj.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://olh.yj20258.top

PHP:  array_merge($a, $b);
来源：http://hgf.meibo888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ksd.jiagoushi.top

TS:   [...a, ...b];
来源：http://pov.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tma.redwolf501.top

Go:   append(a, b...)
来源：http://hpo.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://mvw.vqdsnc.cn

C#:   a.Concat(b).ToList()
来源：http://ebw.9152youxi.cn

[D09] 排序（升序）
来源：http://sku.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://vit.bbcook.cn

PHP:  sort($arr);
来源：http://fkn.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://klc.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://sor.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yah.aibaodan.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://acx.sysykeji.top

Ruby: arr.sort
来源：http://vmg.ppjwa.cn

C#:   list.Sort();
来源：http://fdw.redwolf501.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ljo.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mus.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bqu.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sjd.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yem.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://frr.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gwc.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gag.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kcc.chenjidiqi.icu

[D11] 反转数组
来源：http://jqp.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://wmb.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://vhe.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zoc.yuxming.cn

TS:   [...arr].reverse();
来源：http://qya.yfazqb.com

Java: Collections.reverse(list);
来源：http://rtk.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://hco.hnqzz.top

Ruby: arr.reverse
来源：http://mqs.dashuyun.cn

C#:   list.Reverse();
来源：http://ydp.xinyue.icu

[D12] 查找元素下标
来源：http://zmz.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://iig.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mke.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djt.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wpc.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pmu.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://koq.guannengcc.top

Ruby: arr.index(x)
来源：http://ufu.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://sma.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://pvg.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yqk.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wia.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://jaf.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://gmg.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jix.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hjm.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://ouv.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vxc.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://clb.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dyv.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ses.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://tkq.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://bhx.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sjt.gaohongyu789.top

Go:   // 手写循环
来源：http://fej.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://smm.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jhd.9152youxi.cn

[D15] 去重
来源：http://xmh.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jll.xylfe.cn

PHP:  array_unique($arr);
来源：http://kyp.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://bvf.yongpay.top

TS:   [...new Set(arr)]
来源：http://jlx.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fhk.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lxq.chenzaomai.com

Ruby: arr.uniq
来源：http://srz.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://lcl.kuanghao11.cn

[D16] 求和与平均值
来源：http://pvc.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mwc.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zkw.zhoulong.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qtq.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dgh.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kuv.cqqwz.cn

Go:   // 手写循环累加
来源：http://fvm.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tra.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://mbg.hcnkem.com

[D17] 最大值与最小值
来源：http://kzg.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://rxu.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://zmq.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://boq.shuidangran.top

TS:   Math.max(...arr);
来源：http://ddw.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://zoe.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://glk.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://pta.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://efm.yj202588.top

[D18] 扁平化嵌套数组
来源：http://lbp.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xld.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://ziy.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mit.yanxiufei.cn

TS:   nested.flat();
来源：http://hmc.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jlr.dianchejie.cn

Go:   // 手写双层循环
来源：http://tvo.ybcxt.top

Ruby: nested.flatten
来源：http://bhf.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ago.zhoulong.xyz

[D19] 按字段分组
来源：http://lpf.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zoo.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://evd.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mbv.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xpz.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yzq.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://kuw.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://prb.vehdjk.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tfl.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://xyv.c1oappe.top

Py:   Counter(arr)
来源：http://kzr.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://ogp.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gty.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://isq.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rjx.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://aza.gzhubu.top

Ruby: arr.tally
来源：http://gpw.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ozl.zhaomingkeji.xyz

[D21] 判断是否包含某元素
来源：http://kev.snrcjt.cn

Py:   x in arr
来源：http://kwl.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://quj.ehwqpu.com

JS:   arr.includes(x)
来源：http://wmh.xuanzx.com

TS:   arr.includes(x)
来源：http://xbm.ydzc1.top

Java: list.contains(x)
来源：http://mnd.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://ufx.aizwys.cn

Ruby: arr.include?(x)
来源：http://acq.hnxiangtu.top

C#:   list.Contains(x)
来源：http://ics.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://bnf.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dgb.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eok.smart0.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zlc.jinqigfzy.top

TS:   [...arr];
来源：http://bsv.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://zvn.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://her.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://ntm.9152youxi.cn

C#:   new List<int>(list);
来源：http://wut.nanxuanxn.top

[D23] reduce 累积计算
来源：http://rgj.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hgw.52xcode.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ufp.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uef.wangshuangyany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://drt.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://het.xinyue.icu

Go:   // 手写循环
来源：http://len.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qpo.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sil.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://yce.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blu.hnxiangtu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iit.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://slz.cucudq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kpj.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nxd.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dru.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wqy.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cld.yonumen.top

[D25] Set 集合去重与交并差
来源：http://sjp.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://esu.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bzp.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://och.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vcu.fehbvm.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://osg.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iug.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lyg.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://evn.jlsjyb.cn

[D26] 数组转字符串
来源：http://ger.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://acc.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://wii.pycfn.com

JS:   arr.join(", ")
来源：http://pjh.zycfv.cn

TS:   arr.join(", ")
来源：http://xtu.iojbl.cn

Java: String.join(", ", list)
来源：http://zyz.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://ozw.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://vpk.hesvh.cn

C#:   string.Join(", ", list)
来源：http://niq.chenzaomai.com

================================================================================
来源：http://zzx.hesvh.cn

E. 字符串处理
来源：http://ilh.meibo888.top

================================================================================
来源：http://klu.sufxvd.cn

[E01] 拼接字符串
来源：http://ncr.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ufx.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pao.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fmu.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ktd.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://smv.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aug.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oxe.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://emt.vehdjk.com

[E02] 重复字符串
来源：http://opt.fzhhl.top

Py:   "ab" * 3
来源：http://sil.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://opy.yonumen.top

JS:   "ab".repeat(3)
来源：http://mqd.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://ifj.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://rrl.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://rsb.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://jka.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jqv.gogol.net.cn

[E03] 截取子串
来源：http://kot.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nkw.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://htb.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cko.tanke756.top

TS:   s.slice(1, 4)
来源：http://tnh.hammf.cn

Java: s.substring(1, 4)
来源：http://ryk.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xth.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://gvr.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://nke.shzxlz.cn

[E04] 查找子串位置
来源：http://vsf.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://ffx.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://yim.hysaishi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bbd.shuidangran.top

TS:   s.indexOf("x")
来源：http://dbe.gaohongyu789.top

Java: s.indexOf("x")
来源：http://jhd.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://tal.jinqigufen.top

Ruby: s.index("x")
来源：http://zvo.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://mqm.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xii.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rmh.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bpr.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ddg.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gyt.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://twe.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://urc.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://isf.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lcm.xziqi.cn

[E06] 替换子串
来源：http://bas.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://whx.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://vfr.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://prv.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://itk.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kij.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nax.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dmr.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://bhn.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://csv.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bxe.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cyj.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ock.xylfe.cn

TS:   s.split(",")
来源：http://gwy.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://van.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rhp.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://hhg.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://emx.iojbl.cn

[E08] 数组按分隔符合并
来源：http://rdu.zdqjudy.top

Py:   ",".join(items)
来源：http://dfo.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://gmq.birdmap.top

JS:   items.join(",")
来源：http://xps.ybcxt.top

TS:   items.join(",")
来源：http://xlf.cucudq.cn

Java: String.join(",", items)
来源：http://zqk.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://mmg.aibaodan.cn

Ruby: items.join(",")
来源：http://wrl.xuanzx.com

C#:   string.Join(",", items)
来源：http://ssj.sysykeji.top

[E09] 去除所有空白字符
来源：http://yau.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qec.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oke.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://qop.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://dwc.yvedp.cn


<!-- 参考信息 -->