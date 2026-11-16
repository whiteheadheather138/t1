代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qna.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rzf.havefunace.top

[D05] 访问与修改元素
来源：http://mta.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lwa.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dkn.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://grj.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://nxf.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://vkk.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://zto.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://epr.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://stn.yj20258888.top

[D06] 数组长度
来源：http://mqa.zdbjq.cn

Py:   len(arr)
来源：http://kyp.ctjpmb.com

PHP:  count($arr);
来源：http://xmy.zycfv.cn

JS:   arr.length
来源：http://svm.zycfv.cn

TS:   arr.length
来源：http://lkj.snrcjt.cn

Java: list.size();
来源：http://mor.sxryk.cn

Go:   len(arr)
来源：http://vtc.xinyue.icu

Ruby: arr.length; arr.size
来源：http://rik.vqdsnc.cn

C#:   list.Count;
来源：http://lhk.vehdjk.com

[D07] 切片 / 取子数组
来源：http://gss.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dwc.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ykv.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://uzj.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://uvc.chenjidiqi.icu

Java: list.subList(1, 4);
来源：http://ssl.gogol.net.cn

Go:   arr[1:4]
来源：http://jpi.yuxming.cn

Ruby: arr[1, 3]
来源：http://yvn.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://kcl.shuidangran.top

[D08] 合并两个数组
来源：http://iun.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://uir.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://rrb.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hrh.xylfe.cn

TS:   [...a, ...b];
来源：http://iax.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xus.ybcxt.top

Go:   append(a, b...)
来源：http://bck.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://xqp.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://mjf.vehdjk.com

[D09] 排序（升序）
来源：http://lvv.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://sss.shzxlz.cn

PHP:  sort($arr);
来源：http://zkj.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ivn.yangfankeji.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://uwp.zhongyouzk.top

Java: Collections.sort(list);  list.sort(null);
来源：http://itr.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ige.shangyingyoupin.top

Ruby: arr.sort
来源：http://tvv.yonumen.top

C#:   list.Sort();
来源：http://njo.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://enk.shanyushiyangtech.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lgp.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cwq.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oyf.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://okg.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lut.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tmy.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://klt.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cse.ydjk.org.cn

[D11] 反转数组
来源：http://cji.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://uec.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://nht.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wbj.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://art.cheryme.top

Java: Collections.reverse(list);
来源：http://ewk.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://bgx.yuanzhike.top

Ruby: arr.reverse
来源：http://imj.yvedp.cn

C#:   list.Reverse();
来源：http://jju.daxiang520.top

[D12] 查找元素下标
来源：http://fpp.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://gpj.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fla.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://urz.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rkg.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kgd.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://mqf.hcnkem.com

Ruby: arr.index(x)
来源：http://lsx.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://flt.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://mqm.fengsongda.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pfz.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tym.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://pcb.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://fdc.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mxq.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://myg.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://axp.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://shh.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://ugt.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zki.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oam.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://imy.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://nqd.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://oau.meibo888.top

Go:   // 手写循环
来源：http://dze.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://jpp.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://whw.shanyushiyangtech.top

[D15] 去重
来源：http://tpg.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iug.xuanzx.com

PHP:  array_unique($arr);
来源：http://esg.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://ogb.pycfn.com

TS:   [...new Set(arr)]
来源：http://diu.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sxd.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://ugp.pycfn.com

Ruby: arr.uniq
来源：http://eux.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://akh.gaohongyu789.top

[D16] 求和与平均值
来源：http://bzf.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jze.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fui.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vcv.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qey.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mly.yj202588.top

Go:   // 手写循环累加
来源：http://hcj.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ruz.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://dfh.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://hhw.tanke756.top

Py:   max(arr);  min(arr)
来源：http://xyx.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://ohu.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vzl.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://ixx.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://koe.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pja.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://ypp.jyoumei.cn

C#:   list.Max();  list.Min()
来源：http://gxg.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://rbh.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ksj.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://rej.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nnr.pycfn.com

TS:   nested.flat();
来源：http://ukb.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pov.zhongyouzk.top

Go:   // 手写双层循环
来源：http://kff.jqgufenzy.top

Ruby: nested.flatten
来源：http://jyw.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uyt.yongpay.top

[D19] 按字段分组
来源：http://sgk.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sbu.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yek.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xeg.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://cas.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wqz.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://hmh.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xve.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sif.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://ztw.ydzc1.top

Py:   Counter(arr)
来源：http://mxt.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://zhm.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tmn.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ptp.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ben.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://yuy.pengpengdd.cyou

Ruby: arr.tally
来源：http://krh.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dzg.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://vmz.pycfn.com

Py:   x in arr
来源：http://bmk.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://gzs.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://qqj.yuxming.cn

TS:   arr.includes(x)
来源：http://sem.fzhhl.top

Java: list.contains(x)
来源：http://hbv.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://lge.yvedp.cn

Ruby: arr.include?(x)
来源：http://ldp.xziqi.cn

C#:   list.Contains(x)
来源：http://sco.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://ayq.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://orh.fanxiaobao.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xju.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qdv.tarul.cn

TS:   [...arr];
来源：http://plf.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://sgb.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://uvs.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://bvi.daxiang520.top

C#:   new List<int>(list);
来源：http://xvl.hcnkem.com

[D23] reduce 累积计算
来源：http://pkj.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uls.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ulr.pycfn.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uzs.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cjr.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ttb.hongshengwenyu.top

Go:   // 手写循环
来源：http://sua.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://och.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bun.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://ewr.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hcp.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rlb.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wpw.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://naa.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qxk.shangyingyoupin.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gbm.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vrz.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bvs.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://noa.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dab.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://khr.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mvp.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hhw.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qlj.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://owg.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xpj.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://reg.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://szz.hnxiangtu.top

Py:   ", ".join(map(str, arr))
来源：http://yps.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://ijc.daxiang520.top

JS:   arr.join(", ")
来源：http://nzj.uphjek.com

TS:   arr.join(", ")
来源：http://hom.zhengqikj.top

Java: String.join(", ", list)
来源：http://xgd.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://amy.zdbjq.cn

Ruby: arr.join(", ")
来源：http://twm.shuidangran.top

C#:   string.Join(", ", list)
来源：http://zxk.birdmap.top

================================================================================
来源：http://fjy.ehwqpu.com

E. 字符串处理
来源：http://fsq.quarkkingdee.top

================================================================================
来源：http://xan.wangdashe.top

[E01] 拼接字符串
来源：http://cml.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://imu.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sfg.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yrj.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfq.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://irn.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mdg.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oiv.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bkg.sysykeji.top

[E02] 重复字符串
来源：http://szx.fktsv.cn

Py:   "ab" * 3
来源：http://lqb.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://vdo.yongpay.top

JS:   "ab".repeat(3)
来源：http://lbd.vehdjk.com

TS:   "ab".repeat(3)
来源：http://res.dashuyun.cn

Java: "ab".repeat(3)
来源：http://rvl.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://lyk.uphjek.com

Ruby: "ab" * 3
来源：http://tso.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gbn.haohaochexian.top

[E03] 截取子串
来源：http://pbj.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ull.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rma.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hax.xuanzx.com

TS:   s.slice(1, 4)
来源：http://wvz.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://vsg.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://soo.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ibk.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://tre.tianlin.xyz

[E04] 查找子串位置
来源：http://gmf.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://rhd.ydzc1.top

PHP:  strpos($s, "x");
来源：http://lbb.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pho.birdmap.top

TS:   s.indexOf("x")
来源：http://aqu.ydzc1.top

Java: s.indexOf("x")
来源：http://hjh.tarul.cn

Go:   strings.Index(s, "x")
来源：http://mpe.cheryme.top

Ruby: s.index("x")
来源：http://ooy.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://kqu.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qce.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wrz.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aes.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lkg.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qdi.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://odx.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hvh.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kuh.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ztq.vehdjk.com

[E06] 替换子串
来源：http://uve.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hks.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ebu.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jie.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://dwl.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cqa.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ibe.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://shf.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://oud.yuxming.cn

[E07] 按分隔符拆分
来源：http://iuq.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nst.zhaomingkeji.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bvb.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cbb.fanxiaobao.xyz

TS:   s.split(",")
来源：http://zsr.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://quj.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ecg.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://owb.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ncc.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://wlo.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://zez.hammf.cn

PHP:  implode(",", $items);
来源：http://daz.xziqi.cn

JS:   items.join(",")
来源：http://gnq.fengsongda.top

TS:   items.join(",")
来源：http://kwe.zdbjq.cn

Java: String.join(",", items)
来源：http://wax.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://pof.yanxiufei.cn

Ruby: items.join(",")
来源：http://mpp.bjfxy.top

C#:   string.Join(",", items)
来源：http://qoh.cqqwz.cn

[E09] 去除所有空白字符
来源：http://kos.sjlbkw.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bzd.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oxr.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://dci.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://zpt.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://mjc.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cxu.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://hrw.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xbd.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://ich.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aow.tarul.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yob.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://khv.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://oqu.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://epv.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eqd.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ynp.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tmo.nanxinkj.top

[E11] 反转字符串
来源：http://ank.snrcjt.cn

Py:   s[::-1]
来源：http://rzn.birdmap.top

PHP:  strrev($s);
来源：http://hsj.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://ghj.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://ujg.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://muz.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wey.hysaishi.cn


<!-- 参考信息 -->