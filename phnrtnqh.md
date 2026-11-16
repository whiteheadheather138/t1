代发 wailian999

Py:   len(arr)
来源：http://kqi.vehdjk.com

PHP:  count($arr);
来源：http://xjo.daxiang520.top

JS:   arr.length
来源：http://dmd.ivvv.top

TS:   arr.length
来源：http://nrm.hcnkem.com

Java: list.size();
来源：http://lug.zycfv.cn

Go:   len(arr)
来源：http://gdn.cheryme.top

Ruby: arr.length; arr.size
来源：http://kid.ywan-chungtsiang.top

C#:   list.Count;
来源：http://igf.hammf.cn

[D07] 切片 / 取子数组
来源：http://hjx.pycfn.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tsp.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hqr.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://xru.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://bit.9152youxi.cn

Java: list.subList(1, 4);
来源：http://lht.9152youxi.cn

Go:   arr[1:4]
来源：http://uyp.shzxlz.cn

Ruby: arr[1, 3]
来源：http://oie.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://qtw.tarul.cn

[D08] 合并两个数组
来源：http://zcz.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://crf.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://bub.yueranfly.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cen.c1oappe.top

TS:   [...a, ...b];
来源：http://gzy.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mri.zycfv.cn

Go:   append(a, b...)
来源：http://nfc.gzhubu.top

Ruby: a + b;  a.concat(b)
来源：http://uio.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://cty.jqgfzy.top

[D09] 排序（升序）
来源：http://txh.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://wzj.redwolf501.top

PHP:  sort($arr);
来源：http://dqh.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zye.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pmn.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lsx.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ddg.vqdsnc.cn

Ruby: arr.sort
来源：http://tzj.fktsv.cn

C#:   list.Sort();
来源：http://oxq.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vpd.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://agk.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jny.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qob.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cxl.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jto.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cke.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pce.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lrw.kuanghao11.cn

[D11] 反转数组
来源：http://mdw.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://mtr.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://xkh.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vob.ctjpmb.com

TS:   [...arr].reverse();
来源：http://qkz.zycfv.cn

Java: Collections.reverse(list);
来源：http://bsr.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://kmq.bbcook.cn

Ruby: arr.reverse
来源：http://ldd.iojbl.cn

C#:   list.Reverse();
来源：http://xhn.52xcode.cn

[D12] 查找元素下标
来源：http://vqn.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://ikr.ydzc1.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rlv.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pfk.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bde.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aau.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://scj.yonumen.top

Ruby: arr.index(x)
来源：http://frj.daria6918.cn

C#:   list.IndexOf(x);
来源：http://ioc.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://oat.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ylc.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nxw.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://mwa.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://oqx.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ydv.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lvi.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gol.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://cbk.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://jmi.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dih.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xfl.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://mxu.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://hdl.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ztl.hnqzz.top

Go:   // 手写循环
来源：http://xid.guannengcc.top

Ruby: arr.map { |x| x * 2 }
来源：http://ait.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vjb.yvedp.cn

[D15] 去重
来源：http://zen.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ilj.sufxvd.cn

PHP:  array_unique($arr);
来源：http://gly.havefunace.top

JS:   [...new Set(arr)]
来源：http://ndh.hcnkem.com

TS:   [...new Set(arr)]
来源：http://jvc.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://myd.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://jdm.tianlin.xyz

Ruby: arr.uniq
来源：http://adt.meibo888.top

C#:   list.Distinct().ToList()
来源：http://gho.guannengcc.top

[D16] 求和与平均值
来源：http://ium.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iov.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ftt.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://myi.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oso.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lyc.meibo888.top

Go:   // 手写循环累加
来源：http://tek.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lca.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://mfk.ivvv.top

[D17] 最大值与最小值
来源：http://gij.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://hkw.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://lgw.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fmy.fengsongda.top

TS:   Math.max(...arr);
来源：http://wac.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rsu.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gah.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://cvw.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://gax.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://nyg.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hls.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://dft.uphjek.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ykd.fehbvm.com

TS:   nested.flat();
来源：http://egt.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://twq.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://qto.jqgufenzy.top

Ruby: nested.flatten
来源：http://ezu.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sfq.tianlin.xyz

[D19] 按字段分组
来源：http://qak.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vbk.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fdu.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://msa.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cik.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uns.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://pjg.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uoo.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hac.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://evt.gotoacloud.top

Py:   Counter(arr)
来源：http://llt.yvedp.cn

PHP:  array_count_values($arr);
来源：http://krw.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ehj.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zxg.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ton.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://efl.sjlbkw.cn

Ruby: arr.tally
来源：http://sle.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hhx.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://dzc.meibo888.top

Py:   x in arr
来源：http://cuo.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://jpz.xuanzx.com

JS:   arr.includes(x)
来源：http://bye.dashuyun.cn

TS:   arr.includes(x)
来源：http://ixk.bbcook.cn

Java: list.contains(x)
来源：http://yhb.cqqwz.cn

Go:   slices.Contains(arr, x)
来源：http://xri.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://ozb.smart0.xyz

C#:   list.Contains(x)
来源：http://mbj.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://epx.ybcxt.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ryc.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gth.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ugy.nanxuanxn.top

TS:   [...arr];
来源：http://pdh.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://ylj.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://hqz.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://hrn.gaohongyu789.top

C#:   new List<int>(list);
来源：http://kuu.xziqi.cn

[D23] reduce 累积计算
来源：http://yxl.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fvu.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ldh.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wff.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://deq.zhongyouzk.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dxj.hongshengwenyu.top

Go:   // 手写循环
来源：http://wgo.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zgk.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nmo.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://vyg.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uyw.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mif.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://odl.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uye.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dbs.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xkq.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lvl.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hsr.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://tfu.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hhl.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://anh.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dax.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aio.chenlongwang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ndq.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ahv.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bbs.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tnm.havefunace.top

[D26] 数组转字符串
来源：http://ugs.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://eva.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://vvl.fzhhl.top

JS:   arr.join(", ")
来源：http://mev.yangfankeji.com

TS:   arr.join(", ")
来源：http://jpl.zhixingplan.top

Java: String.join(", ", list)
来源：http://rif.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://rps.jianghu66.top

Ruby: arr.join(", ")
来源：http://ixr.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://iiw.zdqjudy.top

================================================================================
来源：http://aip.redwolf501.top

E. 字符串处理
来源：http://mln.zhaomingkeji.xyz

================================================================================
来源：http://qwp.yongpay.top

[E01] 拼接字符串
来源：http://fkr.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gzj.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hzz.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ajn.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lpp.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hct.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kem.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yzx.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kje.aizwys.cn

[E02] 重复字符串
来源：http://cij.gotoacloud.top

Py:   "ab" * 3
来源：http://dut.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://pyc.yj20258.top

JS:   "ab".repeat(3)
来源：http://vqr.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://gyi.316326.xyz

Java: "ab".repeat(3)
来源：http://nec.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://txp.havefunace.top

Ruby: "ab" * 3
来源：http://qtg.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://upb.cashguo.top

[E03] 截取子串
来源：http://efo.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sep.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lep.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nkg.meibo888.top

TS:   s.slice(1, 4)
来源：http://gbn.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://ocs.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ycw.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dmf.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://scg.havefunace.top

[E04] 查找子串位置
来源：http://fhr.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://eid.mhx1999.top

PHP:  strpos($s, "x");
来源：http://uxg.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rgh.smart0.xyz

TS:   s.indexOf("x")
来源：http://wgs.smart0.xyz

Java: s.indexOf("x")
来源：http://deu.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://kqw.yj202588.top

Ruby: s.index("x")
来源：http://guy.ppjwa.cn

C#:   s.IndexOf("x")
来源：http://syl.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ucz.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hff.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mcg.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zwu.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kty.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nqv.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ffv.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tuv.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zdz.yonumen.top

[E06] 替换子串
来源：http://kkt.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wkh.jyoumei.cn

PHP:  str_replace("a", "b", $s);
来源：http://wkn.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fsm.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://rqr.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jaq.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xnj.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bki.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://nkb.tarul.cn

[E07] 按分隔符拆分
来源：http://ozu.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xiy.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hvf.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lde.haohaochexian.top

TS:   s.split(",")
来源：http://oqo.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://fbm.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jso.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://yzi.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xjy.fzhhl.top

[E08] 数组按分隔符合并
来源：http://yiw.tanke756.top

Py:   ",".join(items)
来源：http://pfe.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://zcc.0kj1m.cn

JS:   items.join(",")
来源：http://fze.svipenyu.cn

TS:   items.join(",")
来源：http://oci.c1oappe.top

Java: String.join(",", items)
来源：http://qtv.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://jcd.hnxiangtu.top

Ruby: items.join(",")
来源：http://oej.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://ifa.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://bbz.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dun.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fky.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://hgm.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://pxy.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://wmu.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://gxq.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://duv.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vvx.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://pky.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vbw.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://khm.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://spi.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://jem.yongpay.top

Java: String.format("%03d", 7)
来源：http://xrc.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ymt.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uwu.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qbi.shzxlz.cn

[E11] 反转字符串
来源：http://tnp.shanyushiyangtech.top

Py:   s[::-1]
来源：http://ucc.yj20258888.top

PHP:  strrev($s);
来源：http://ufa.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://wsc.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://pvv.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://wbt.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://sux.yueranfly.top

Ruby: s.reverse
来源：http://zej.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qhl.bbcook.cn

[E12] 统计某字符出现次数
来源：http://hzf.quarkkingdee.top

Py:   s.count("a")
来源：http://qtk.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://gdd.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://foy.bbcook.cn

TS:   s.split("a").length - 1
来源：http://ehd.ctjpmb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xuj.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://ixl.cqqwz.cn

Ruby: s.count("a")
来源：http://qyx.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://jjl.xziqi.cn

[E13] 逐字符遍历
来源：http://mud.tianlin.xyz


<!-- 参考信息 -->