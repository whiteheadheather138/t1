代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gxi.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://ter.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ntv.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gnx.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ftc.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bkv.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://ium.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jxw.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mmp.shzxlz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aps.jianghu66.top

TS:   arr[0]; arr.at(-1);
来源：http://xdb.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://rcf.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ezr.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bag.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qgq.hysaishi.cn

[D06] 数组长度
来源：http://rdh.tanke756.top

Py:   len(arr)
来源：http://ywl.dashuyun.cn

PHP:  count($arr);
来源：http://emc.xziqi.cn

JS:   arr.length
来源：http://mzx.jinqigfzy.top

TS:   arr.length
来源：http://muk.yonumen.top

Java: list.size();
来源：http://lgj.yvedp.cn

Go:   len(arr)
来源：http://awf.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://kjk.jinghuilouyu.cn

C#:   list.Count;
来源：http://nyc.fehbvm.com

[D07] 切片 / 取子数组
来源：http://ong.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ufa.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bbs.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://kwk.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://auw.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://pau.shangyingyoupin.top

Go:   arr[1:4]
来源：http://zkj.tian-w.cn

Ruby: arr[1, 3]
来源：http://fzg.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://rtm.xziqi.cn

[D08] 合并两个数组
来源：http://rcz.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://wqj.bjfxy.top

PHP:  array_merge($a, $b);
来源：http://hid.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vpf.jlsjyb.cn

TS:   [...a, ...b];
来源：http://piy.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hhr.epnwcf.com

Go:   append(a, b...)
来源：http://enl.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://hcs.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://cpm.kuanghao11.cn

[D09] 排序（升序）
来源：http://yxa.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://edr.pengpengdd.cyou

PHP:  sort($arr);
来源：http://ejp.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://arq.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://taw.epnwcf.com

Java: Collections.sort(list);  list.sort(null);
来源：http://pbo.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yjs.yj20258888.top

Ruby: arr.sort
来源：http://gso.aizwys.cn

C#:   list.Sort();
来源：http://dim.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tkr.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pzx.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lnl.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tuj.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zbx.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xzd.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://squ.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://air.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://prs.gotoacloud.top

[D11] 反转数组
来源：http://yjk.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wcj.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://zos.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gij.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://foq.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://ant.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://kre.fktsv.cn

Ruby: arr.reverse
来源：http://shx.ydzc1.top

C#:   list.Reverse();
来源：http://jae.cashguo.top

[D12] 查找元素下标
来源：http://qmr.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://qsb.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pnt.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://web.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dyy.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ptv.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://byf.birdmap.top

Ruby: arr.index(x)
来源：http://fhu.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://iil.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://svq.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ucf.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ebi.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://evj.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://oky.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mul.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pab.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://fuj.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xtc.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://fzd.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://olc.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jpn.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://rjm.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://sir.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ibr.aizwys.cn

Go:   // 手写循环
来源：http://vaf.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://lgt.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://ddo.bjfxy.top

[D15] 去重
来源：http://eja.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nkf.zdqjudy.top

PHP:  array_unique($arr);
来源：http://stm.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://dkt.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://kno.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ntn.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://lcr.ydzc1.top

Ruby: arr.uniq
来源：http://gkq.cashguo.top

C#:   list.Distinct().ToList()
来源：http://szm.gogol.net.cn

[D16] 求和与平均值
来源：http://wwa.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fax.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xvx.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zpf.andypj.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://muj.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vrd.ydzc1.top

Go:   // 手写循环累加
来源：http://itl.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://orw.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://xqt.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://cuz.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://dsi.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://nuj.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://opu.yonumen.top

TS:   Math.max(...arr);
来源：http://dzt.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jxm.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://feg.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://nei.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://eku.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://tvk.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xhg.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://mzz.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hrq.nanxuanxn.top

TS:   nested.flat();
来源：http://nas.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kuf.cashguo.top

Go:   // 手写双层循环
来源：http://aqc.sufxvd.cn

Ruby: nested.flatten
来源：http://kwp.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lha.ybcxt.top

[D19] 按字段分组
来源：http://cec.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kpq.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rel.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ddh.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yie.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://paf.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://diq.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vna.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://atz.yongpay.top

[D20] 统计每个元素出现次数
来源：http://jzq.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://pry.fzhhl.top

PHP:  array_count_values($arr);
来源：http://zag.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pko.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vdv.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ksj.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://bos.guowangkeji.top

Ruby: arr.tally
来源：http://cud.yonumen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pdw.hcnkem.com

[D21] 判断是否包含某元素
来源：http://oib.wangshuangyany.cn

Py:   x in arr
来源：http://kmq.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://rcd.vehdjk.com

JS:   arr.includes(x)
来源：http://xtn.dashuyun.cn

TS:   arr.includes(x)
来源：http://lra.pengpengdd.cyou

Java: list.contains(x)
来源：http://bjb.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://anl.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://tst.sysykeji.top

C#:   list.Contains(x)
来源：http://iqg.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://azx.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yda.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mke.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://amm.ywan-chungtsiang.top

TS:   [...arr];
来源：http://tsc.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://pid.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://szo.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://gpa.ivvv.top

C#:   new List<int>(list);
来源：http://vji.dianchejie.cn

[D23] reduce 累积计算
来源：http://dtf.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ckq.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hxy.kuanghao11.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lib.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gsi.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qev.hysaishi.cn

Go:   // 手写循环
来源：http://ruj.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pcp.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://owp.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://qwx.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mlw.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wdj.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wyo.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://izk.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ate.nanxuanxn.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dbt.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wth.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gry.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://lit.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rty.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gkz.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bsv.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ikq.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gwe.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vhj.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vnu.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qqw.tanke756.top

[D26] 数组转字符串
来源：http://eya.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://huw.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://sdc.jyoumei.cn

JS:   arr.join(", ")
来源：http://qfy.ydjk.org.cn

TS:   arr.join(", ")
来源：http://lpi.gzhubu.top

Java: String.join(", ", list)
来源：http://lif.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://rti.daria6918.cn

Ruby: arr.join(", ")
来源：http://bmu.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://kwu.havefunace.top

================================================================================
来源：http://thb.tianlin.xyz

E. 字符串处理
来源：http://jgj.hammf.cn

================================================================================
来源：http://epr.jianghu66.top

[E01] 拼接字符串
来源：http://ayi.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mjo.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bjl.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wbw.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aak.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ana.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tin.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vpb.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cst.hesvh.cn

[E02] 重复字符串
来源：http://xjh.shzxlz.cn

Py:   "ab" * 3
来源：http://xix.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://vnp.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://ojb.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://suq.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://rwn.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://zew.snrcjt.cn

Ruby: "ab" * 3
来源：http://sqj.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ygm.yonumen.top

[E03] 截取子串
来源：http://bxm.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dph.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jjw.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jmn.yueranfly.top

TS:   s.slice(1, 4)
来源：http://tcc.fehbvm.com

Java: s.substring(1, 4)
来源：http://okb.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cfe.0kj1m.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ngk.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://hyv.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://ysy.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://vjv.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://tvm.cashguo.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zng.hesvh.cn

TS:   s.indexOf("x")
来源：http://oet.xuanzx.com

Java: s.indexOf("x")
来源：http://jxv.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://rne.hnxiangtu.top

Ruby: s.index("x")
来源：http://pdu.fehbvm.com

C#:   s.IndexOf("x")
来源：http://zzy.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zhb.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://urg.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zzk.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fdd.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://vqh.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ptg.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dvp.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xfa.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://npx.hongshengwenyu.top

[E06] 替换子串
来源：http://yqf.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jzz.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://drx.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iys.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://wse.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jtp.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uzv.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uop.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://dhh.wangdashe.top

[E07] 按分隔符拆分
来源：http://ins.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jst.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bui.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tlt.haohaochexian.top

TS:   s.split(",")
来源：http://qgn.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://azd.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tzd.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://ljj.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wju.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://mvd.jlsjyb.cn

Py:   ",".join(items)
来源：http://wfe.iojbl.cn

PHP:  implode(",", $items);
来源：http://ftp.yvedp.cn

JS:   items.join(",")
来源：http://paf.bjfxy.top

TS:   items.join(",")
来源：http://aul.feifeiyinyue.top

Java: String.join(",", items)
来源：http://sqa.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://uaq.hnxiangtu.top

Ruby: items.join(",")
来源：http://hfn.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://fzz.daxiang520.top

[E09] 去除所有空白字符
来源：http://arl.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iws.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qsg.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://drh.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://mpk.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://lxk.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qor.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://tss.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vbs.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://ufy.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://adv.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://udb.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://pko.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://cdj.ydzc1.top

Java: String.format("%03d", 7)
来源：http://twj.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xwj.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vzo.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kuc.jqgfzy.top

[E11] 反转字符串
来源：http://dbu.cqqwz.cn

Py:   s[::-1]
来源：http://orx.hfpthk.cn

PHP:  strrev($s);
来源：http://gbq.jinghuilouyu.cn


<!-- 参考信息 -->