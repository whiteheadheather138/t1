代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://fpy.svipenyu.cn

Java: list.add(0, 0);
来源：http://htj.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://awc.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dzd.haohaochexian.top

C#:   list.Insert(0, 0);
来源：http://wjp.nanxuanxn.top

[D04] 删除元素
来源：http://wby.bjfxy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xtc.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xdd.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://afg.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://jgk.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://utk.gzhubu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://exc.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ehq.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dbc.zhoulong.xyz

[D05] 访问与修改元素
来源：http://uuu.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://esw.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hpa.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jgz.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://xct.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://xti.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://hwi.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ksz.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tnb.fktsv.cn

[D06] 数组长度
来源：http://abo.ctjpmb.com

Py:   len(arr)
来源：http://kxs.52xcode.cn

PHP:  count($arr);
来源：http://rrp.zhixingplan.top

JS:   arr.length
来源：http://btq.jinqigufen.top

TS:   arr.length
来源：http://sfv.tianlin.xyz

Java: list.size();
来源：http://oxe.zhoulong.xyz

Go:   len(arr)
来源：http://lda.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://mfz.birdmap.top

C#:   list.Count;
来源：http://pnf.redwolf501.top

[D07] 切片 / 取子数组
来源：http://pma.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qgv.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yfv.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://vad.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://xuw.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://usd.316326.xyz

Go:   arr[1:4]
来源：http://zth.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://hbs.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://bht.ivvv.top

[D08] 合并两个数组
来源：http://lil.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://mxm.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://hvl.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bwt.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://xwf.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zlg.fengsongda.top

Go:   append(a, b...)
来源：http://gnv.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://dvb.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://tei.svipenyu.cn

[D09] 排序（升序）
来源：http://hta.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://pht.dashuyun.cn

PHP:  sort($arr);
来源：http://wuc.xingfuxueyuan.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mkf.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wer.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xtq.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hhg.cheryme.top

Ruby: arr.sort
来源：http://jcu.ehwqpu.com

C#:   list.Sort();
来源：http://lwq.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mva.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aeu.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ywn.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zvz.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://adt.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ops.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://afl.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wqc.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ksw.zhaomingkeji.xyz

[D11] 反转数组
来源：http://alt.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://omd.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://nhs.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dqa.mhx1999.top

TS:   [...arr].reverse();
来源：http://arh.hywenlv.cn

Java: Collections.reverse(list);
来源：http://yxw.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://sxl.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://gjr.xuetiantiany.cn

C#:   list.Reverse();
来源：http://xyb.jyoumei.cn

[D12] 查找元素下标
来源：http://mnu.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://ani.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://siv.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tnn.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uvw.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wmg.meibo888.top

Go:   slices.Index(arr, x)
来源：http://xer.ivvv.top

Ruby: arr.index(x)
来源：http://mkz.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://kla.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://ttg.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://apo.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wzs.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://qrc.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://hxv.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qdv.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dob.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://ppm.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lpg.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://hzk.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zlq.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nuc.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://ejs.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://iso.feifeiyinyue.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uvj.yuxming.cn

Go:   // 手写循环
来源：http://pkv.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://ava.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ujf.yonumen.top

[D15] 去重
来源：http://eyt.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rfz.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://qir.redwolf501.top

JS:   [...new Set(arr)]
来源：http://juo.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://xwx.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zdm.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://xya.fzhhl.top

Ruby: arr.uniq
来源：http://aik.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://egp.cdnleiting.top

[D16] 求和与平均值
来源：http://xbv.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aob.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dgp.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dtq.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zss.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rfz.hesvh.cn

Go:   // 手写循环累加
来源：http://dvu.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lzv.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://ebf.yonumen.top

[D17] 最大值与最小值
来源：http://kbg.redwolf501.top

Py:   max(arr);  min(arr)
来源：http://uxt.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://ofh.zhengqikj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sdo.chenlongwang.top

TS:   Math.max(...arr);
来源：http://ijv.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sgj.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gic.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://hdl.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://ufz.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://tar.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rra.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://ccd.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wma.vehdjk.com

TS:   nested.flat();
来源：http://sgq.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://etp.yonumen.top

Go:   // 手写双层循环
来源：http://azj.yongpay.top

Ruby: nested.flatten
来源：http://ohp.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ylf.ybcxt.top

[D19] 按字段分组
来源：http://opv.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uib.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hnz.yueranfly.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ifq.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pdw.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ujf.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://myb.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fsg.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vmg.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://nny.daria6918.cn

Py:   Counter(arr)
来源：http://mxi.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://tmw.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aer.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vkh.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dtl.sweek.top

Go:   // 手写 map[T]int
来源：http://mpd.tarul.cn

Ruby: arr.tally
来源：http://zkt.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ifp.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://lgx.fanxiaobao.xyz

Py:   x in arr
来源：http://aei.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://xoy.snrcjt.cn

JS:   arr.includes(x)
来源：http://ico.xylfe.cn

TS:   arr.includes(x)
来源：http://hgs.gzhubu.top

Java: list.contains(x)
来源：http://ghk.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://dca.ydzc1.top

Ruby: arr.include?(x)
来源：http://msr.nanxinkj.top

C#:   list.Contains(x)
来源：http://tvu.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://xam.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oyp.yanxiufei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uhu.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://syq.0kj1m.cn

TS:   [...arr];
来源：http://gqs.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://xgs.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://rji.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://aem.zycfv.cn

C#:   new List<int>(list);
来源：http://rzr.nanxuanxn.top

[D23] reduce 累积计算
来源：http://isv.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bjf.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ofc.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://noa.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://awf.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zgb.quarkkingdee.top

Go:   // 手写循环
来源：http://fwj.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bhe.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hgz.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://ack.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bxv.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vdb.cheryme.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lqe.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zaw.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jbx.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gzk.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tll.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bhg.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://bnp.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xgq.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://usr.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jsv.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mtj.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jov.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nsb.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zqv.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ehc.iojbl.cn

[D26] 数组转字符串
来源：http://ses.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://fyi.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://inu.yuxming.cn

JS:   arr.join(", ")
来源：http://lpn.fktsv.cn

TS:   arr.join(", ")
来源：http://unh.chenzaomai.com

Java: String.join(", ", list)
来源：http://nkb.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://oqo.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://zpt.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://qnt.shuidangran.top

================================================================================
来源：http://wud.andypj.xyz

E. 字符串处理
来源：http://ydp.jqgfzy.top

================================================================================
来源：http://ubc.ppjwa.cn

[E01] 拼接字符串
来源：http://lsh.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://orw.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://off.jyoumei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://scs.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yhd.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dws.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wht.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nwu.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://opf.9152youxi.cn

[E02] 重复字符串
来源：http://imw.tanke756.top

Py:   "ab" * 3
来源：http://zxx.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://ikl.shuidangran.top

JS:   "ab".repeat(3)
来源：http://eqe.xylfe.cn

TS:   "ab".repeat(3)
来源：http://drq.mhx1999.top

Java: "ab".repeat(3)
来源：http://zbh.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://lls.zdbjq.cn

Ruby: "ab" * 3
来源：http://blp.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nkt.sysykeji.top

[E03] 截取子串
来源：http://tyt.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hus.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bww.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uzu.fktsv.cn

TS:   s.slice(1, 4)
来源：http://enb.shzxlz.cn

Java: s.substring(1, 4)
来源：http://qko.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zgz.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qcz.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://gib.redwolf501.top

[E04] 查找子串位置
来源：http://uyy.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://bmy.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://auy.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fjc.daxiang520.top

TS:   s.indexOf("x")
来源：http://bid.havefunace.top

Java: s.indexOf("x")
来源：http://ivn.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://fhh.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://jeo.redwolf501.top

C#:   s.IndexOf("x")
来源：http://amb.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xli.cdnleiting.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ofv.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rpo.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wwa.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pis.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://owe.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://igu.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pgl.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nml.shanyushiyangkeji.top

[E06] 替换子串
来源：http://qcf.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://njg.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://zlg.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hef.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://zwj.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wnx.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zgl.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xye.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://mku.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://shq.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ivz.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zki.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sbq.quarkkingdee.top

TS:   s.split(",")
来源：http://njm.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://zsa.9152youxi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nmq.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://old.cdnleiting.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://akh.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://ouc.zhoulong.xyz

Py:   ",".join(items)
来源：http://wfv.chenzaomai.com

PHP:  implode(",", $items);
来源：http://hth.wangdashe.top

JS:   items.join(",")
来源：http://jqr.yangfankeji.com

TS:   items.join(",")
来源：http://rbk.yonumen.top

Java: String.join(",", items)
来源：http://cha.havefunace.top

Go:   strings.Join(items, ",")
来源：http://pyb.xuanzx.com

Ruby: items.join(",")
来源：http://ozg.daxiang520.top

C#:   string.Join(",", items)
来源：http://yro.aibaodan.cn

[E09] 去除所有空白字符
来源：http://vdy.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fhh.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sll.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://oce.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://kjl.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://wql.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://rwl.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pqa.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dxi.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://xml.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://svu.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tph.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://oiw.iojbl.cn


<!-- 参考信息 -->