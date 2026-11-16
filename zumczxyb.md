代发 wailian999

Java: list.size();
来源：http://dwk.yj20258888.top

Go:   len(arr)
来源：http://vnc.yuxming.cn

Ruby: arr.length; arr.size
来源：http://ito.shuidangran.top

C#:   list.Count;
来源：http://vez.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://jtu.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fts.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://pbn.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://rph.yj20258.top

TS:   arr.slice(1, 4);
来源：http://ycy.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://xoy.316326.xyz

Go:   arr[1:4]
来源：http://rwl.ehwqpu.com

Ruby: arr[1, 3]
来源：http://gnr.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://edt.smart0.xyz

[D08] 合并两个数组
来源：http://mmf.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://wrg.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://rgg.daxiang520.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kob.yuxming.cn

TS:   [...a, ...b];
来源：http://jnb.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qda.shuidangran.top

Go:   append(a, b...)
来源：http://eiy.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://aoy.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://vvh.cqqwz.cn

[D09] 排序（升序）
来源：http://zrb.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://awf.nanxinkj.top

PHP:  sort($arr);
来源：http://yqc.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dan.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iqs.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kzd.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oou.0kj1m.cn

Ruby: arr.sort
来源：http://uiw.jlsjyb.cn

C#:   list.Sort();
来源：http://vqd.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bsf.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jjw.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ist.mhx1999.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ptm.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyp.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ojv.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jbh.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nlx.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hzo.feifeiyinyue.top

[D11] 反转数组
来源：http://tsh.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://waf.guannengcc.top

PHP:  array_reverse($arr);
来源：http://irb.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://grt.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://plc.dianchejie.cn

Java: Collections.reverse(list);
来源：http://ndo.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://reg.jyoumei.cn

Ruby: arr.reverse
来源：http://jcd.gotoacloud.top

C#:   list.Reverse();
来源：http://wtk.zhixingplan.top

[D12] 查找元素下标
来源：http://kat.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://lgy.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gpm.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://txy.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zan.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tjd.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://vbu.yangfankeji.com

Ruby: arr.index(x)
来源：http://tki.52xcode.cn

C#:   list.IndexOf(x);
来源：http://igs.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://mdh.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sqs.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://waz.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://jgr.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://jam.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://non.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qnv.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://lsx.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sxh.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://ivw.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zhm.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cbe.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://eas.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://huu.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://avu.chenjidiqi.icu

Go:   // 手写循环
来源：http://zno.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://try.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://dew.fengsongda.top

[D15] 去重
来源：http://eyo.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://opq.shzxlz.cn

PHP:  array_unique($arr);
来源：http://ctv.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://chq.sufxvd.cn

TS:   [...new Set(arr)]
来源：http://rad.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wsz.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://idc.fzhhl.top

Ruby: arr.uniq
来源：http://qai.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://tem.hnxiangtu.top

[D16] 求和与平均值
来源：http://oha.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://las.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://say.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mcd.tanke756.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rdu.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uwy.snrcjt.cn

Go:   // 手写循环累加
来源：http://hib.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hkt.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://qcn.sjlbkw.cn

[D17] 最大值与最小值
来源：http://uqo.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://zmi.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://qnh.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ifx.sysykeji.top

TS:   Math.max(...arr);
来源：http://xov.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ogc.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rdv.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://boh.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://irh.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://adf.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xdi.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://bvw.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wka.cashguo.top

TS:   nested.flat();
来源：http://vrl.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qrr.meibo888.top

Go:   // 手写双层循环
来源：http://pxz.meibo888.top

Ruby: nested.flatten
来源：http://bpc.meibo888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mdj.316326.xyz

[D19] 按字段分组
来源：http://zfx.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qrg.jiagoushi.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fpp.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sxt.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dmf.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xif.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://iyw.snrcjt.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://awb.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ffq.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://euj.hfpthk.cn

Py:   Counter(arr)
来源：http://lxf.birdmap.top

PHP:  array_count_values($arr);
来源：http://mml.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sqv.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uyp.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fak.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://gpt.fehbvm.com

Ruby: arr.tally
来源：http://ets.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ugk.fengsongda.top

[D21] 判断是否包含某元素
来源：http://opt.svipenyu.cn

Py:   x in arr
来源：http://zjt.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://xms.ydjk.org.cn

JS:   arr.includes(x)
来源：http://qxi.tanke756.top

TS:   arr.includes(x)
来源：http://uts.cdnleiting.top

Java: list.contains(x)
来源：http://zdq.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://acz.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://mlx.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://btq.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://mou.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mve.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ycw.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vld.quarkkingdee.top

TS:   [...arr];
来源：http://xcg.sweek.top

Java: new ArrayList<>(list);
来源：http://khg.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://koo.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://xmc.jianghu66.top

C#:   new List<int>(list);
来源：http://mnx.nwbrower.top

[D23] reduce 累积计算
来源：http://xrw.iojbl.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ddo.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vni.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nss.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ryn.chenlongwang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bgo.nanxuanxn.top

Go:   // 手写循环
来源：http://tam.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nto.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nmx.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://bga.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jlc.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://asr.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tno.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lfi.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cso.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jcg.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://afc.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fwt.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://ulc.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wfj.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uoo.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vgj.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cvm.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://khh.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zfg.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://btg.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mgk.chenlongwang.top

[D26] 数组转字符串
来源：http://bhs.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://hoi.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://yag.sweek.top

JS:   arr.join(", ")
来源：http://ggg.hnxiangtu.top

TS:   arr.join(", ")
来源：http://ddh.sjlbkw.cn

Java: String.join(", ", list)
来源：http://nvc.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://rws.andypj.xyz

Ruby: arr.join(", ")
来源：http://ptr.yj20258.top

C#:   string.Join(", ", list)
来源：http://mgy.yuxming.cn

================================================================================
来源：http://ojz.cucudq.cn

E. 字符串处理
来源：http://gsh.uphjek.com

================================================================================
来源：http://onr.ydjk.org.cn

[E01] 拼接字符串
来源：http://dhi.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wft.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lqt.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oiw.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zxv.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://och.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yie.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qlr.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mlv.gotoacloud.top

[E02] 重复字符串
来源：http://isa.ehwqpu.com

Py:   "ab" * 3
来源：http://yov.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://fnn.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://fml.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://bej.daxiang520.top

Java: "ab".repeat(3)
来源：http://nhe.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://xcr.pycfn.com

Ruby: "ab" * 3
来源：http://iup.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pra.fehbvm.com

[E03] 截取子串
来源：http://jko.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tjn.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mpx.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vvg.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://xzg.hesvh.cn

Java: s.substring(1, 4)
来源：http://pxx.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hzl.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://wig.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://wgv.gotoacloud.top

[E04] 查找子串位置
来源：http://ydg.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://bxl.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://ssj.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hoj.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://lpl.tanke756.top

Java: s.indexOf("x")
来源：http://lwe.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://meo.zhixingplan.top

Ruby: s.index("x")
来源：http://bbj.zycfv.cn

C#:   s.IndexOf("x")
来源：http://gfj.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://ytv.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jkp.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nks.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xcb.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dmf.hcnkem.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://smr.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pcg.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aas.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yvj.hnxiangtu.top

[E06] 替换子串
来源：http://thr.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tlv.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ijt.zhengqikj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gwa.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://ifv.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://duu.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aqp.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gnk.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://rmk.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://prk.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ahz.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mlk.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ytj.9152youxi.cn

TS:   s.split(",")
来源：http://wct.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://vun.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xnp.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://ahq.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ccu.fktsv.cn

[E08] 数组按分隔符合并
来源：http://zfl.smart0.xyz

Py:   ",".join(items)
来源：http://dyr.andypj.xyz

PHP:  implode(",", $items);
来源：http://qjq.hywenlv.cn

JS:   items.join(",")
来源：http://hpu.vehdjk.com

TS:   items.join(",")
来源：http://gvd.xziqi.cn

Java: String.join(",", items)
来源：http://jkq.sxryk.cn

Go:   strings.Join(items, ",")
来源：http://whe.zdqjudy.top

Ruby: items.join(",")
来源：http://trd.smart0.xyz

C#:   string.Join(",", items)
来源：http://epl.sweek.top

[E09] 去除所有空白字符
来源：http://hel.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kct.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sqf.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://xxj.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://ojk.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://fee.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://faa.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mbx.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tgy.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://czr.jqgufenzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dcz.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vhr.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://wjb.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://xfg.cheryme.top

Java: String.format("%03d", 7)
来源：http://lej.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bte.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mqu.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kgo.wangdashe.top

[E11] 反转字符串
来源：http://rqw.fanxiaobao.xyz

Py:   s[::-1]
来源：http://zgb.bbcook.cn

PHP:  strrev($s);
来源：http://lsr.shanyushiyangtech.top

JS:   [...s].reverse().join("")
来源：http://ndd.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://grh.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ags.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tqj.birdmap.top

Ruby: s.reverse
来源：http://cyn.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qrb.hongshengwenyu.top

[E12] 统计某字符出现次数
来源：http://lhk.hnxiangtu.top

Py:   s.count("a")
来源：http://lwa.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://oqr.yfazqb.com

JS:   s.split("a").length - 1
来源：http://tlp.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://doe.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mrq.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://cgz.hnqzz.top

Ruby: s.count("a")
来源：http://lrn.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://xjx.kuanghao11.cn

[E13] 逐字符遍历
来源：http://fgs.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://nyp.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mtb.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://htk.jianghu66.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cfz.xuetiantiany.cn


<!-- 参考信息 -->