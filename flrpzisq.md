代发 wailian999

[D03] 在指定位置插入元素
来源：http://sbw.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://waa.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rsg.jqgufenzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://quy.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://ggq.fehbvm.com

Java: list.add(0, 0);
来源：http://cdp.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://zsb.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hca.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://zeh.yonumen.top

[D04] 删除元素
来源：http://mpi.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aue.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dme.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ram.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://hfb.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qmf.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gob.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://htp.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://goj.hammf.cn

[D05] 访问与修改元素
来源：http://bfm.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nws.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://quy.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://elh.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://xsg.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://cst.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://qwi.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pjq.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ban.vqdsnc.cn

[D06] 数组长度
来源：http://jpa.cheryme.top

Py:   len(arr)
来源：http://uyx.316326.xyz

PHP:  count($arr);
来源：http://ijs.vqdsnc.cn

JS:   arr.length
来源：http://tei.yonumen.top

TS:   arr.length
来源：http://fct.yj20258888.top

Java: list.size();
来源：http://dpu.cashguo.top

Go:   len(arr)
来源：http://paj.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://yab.guowangkeji.top

C#:   list.Count;
来源：http://ple.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://scb.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ikk.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://uso.yj20258.top

JS:   arr.slice(1, 4);
来源：http://akl.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://ddo.hfpthk.cn

Java: list.subList(1, 4);
来源：http://lyb.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://fsj.c1oappe.top

Ruby: arr[1, 3]
来源：http://xxl.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://eef.xinyue.icu

[D08] 合并两个数组
来源：http://yod.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://qzo.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://acy.ppjwa.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yko.cucudq.cn

TS:   [...a, ...b];
来源：http://wbv.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://otn.daria6918.cn

Go:   append(a, b...)
来源：http://gvf.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://zxg.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://ezu.yuxming.cn

[D09] 排序（升序）
来源：http://oay.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://cxj.yuanzhike.top

PHP:  sort($arr);
来源：http://zzs.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oiv.smart0.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ghd.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yyb.yfazqb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dlp.nwbrower.top

Ruby: arr.sort
来源：http://akh.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://yyb.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eom.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zbv.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eva.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://juc.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tyr.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kji.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pjp.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cve.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fhj.zycfv.cn

[D11] 反转数组
来源：http://qpm.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://juy.fengsongda.top

PHP:  array_reverse($arr);
来源：http://jzb.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://twy.havefunace.top

TS:   [...arr].reverse();
来源：http://byz.xinyue.icu

Java: Collections.reverse(list);
来源：http://fwp.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://jkn.zhixingplan.top

Ruby: arr.reverse
来源：http://jhr.jyoumei.cn

C#:   list.Reverse();
来源：http://gky.yangfankeji.com

[D12] 查找元素下标
来源：http://kiy.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://toc.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dbg.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sxf.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xkz.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://juc.yj202588.top

Go:   slices.Index(arr, x)
来源：http://tga.yj202588.top

Ruby: arr.index(x)
来源：http://skr.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://tpb.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://ngk.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sbx.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vuu.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://zew.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://lxf.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qdy.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qls.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://rxf.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vzz.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://uhu.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ytz.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cmy.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://doi.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://jhz.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jhr.svipenyu.cn

Go:   // 手写循环
来源：http://uwg.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://yib.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yqz.hongshengwenyu.top

[D15] 去重
来源：http://gsi.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zwg.fanxiaobao.xyz

PHP:  array_unique($arr);
来源：http://qam.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://qgk.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://iop.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qus.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://gwu.xinyue.icu

Ruby: arr.uniq
来源：http://jen.316326.xyz

C#:   list.Distinct().ToList()
来源：http://cwj.hfpthk.cn

[D16] 求和与平均值
来源：http://ony.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sdt.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pea.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zzk.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ooz.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://emg.kuanghao11.cn

Go:   // 手写循环累加
来源：http://fbs.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mzs.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://nmt.yuanzhike.top

[D17] 最大值与最小值
来源：http://ydf.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://mxt.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://qdc.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://doh.xziqi.cn

TS:   Math.max(...arr);
来源：http://jtk.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jlh.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lzi.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://zdl.xziqi.cn

C#:   list.Max();  list.Min()
来源：http://exu.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://obe.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qzx.uphjek.com

PHP:  array_merge(...$nested);
来源：http://vea.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xhk.sjlbkw.cn

TS:   nested.flat();
来源：http://ogk.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qgf.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://cgc.gaohongyu789.top

Ruby: nested.flatten
来源：http://jtl.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://rfz.xinyue.icu

[D19] 按字段分组
来源：http://ekf.cashguo.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hol.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gma.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hue.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jdx.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://icu.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://rmh.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://thp.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zcg.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://whf.hysaishi.cn

Py:   Counter(arr)
来源：http://fos.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://dxl.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jmu.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oqt.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rmr.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://nay.jinqigfzy.top

Ruby: arr.tally
来源：http://ckf.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gdp.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://wew.fehbvm.com

Py:   x in arr
来源：http://dvv.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://xua.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://uej.mhx1999.top

TS:   arr.includes(x)
来源：http://ywz.fzhhl.top

Java: list.contains(x)
来源：http://nkc.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://ufs.ivvv.top

Ruby: arr.include?(x)
来源：http://tkd.quarkkingdee.top

C#:   list.Contains(x)
来源：http://dwv.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://gwe.snrcjt.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ppr.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hnw.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bjc.ybcxt.top

TS:   [...arr];
来源：http://zdw.fengsongda.top

Java: new ArrayList<>(list);
来源：http://smy.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://bto.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://pnz.epnwcf.com

C#:   new List<int>(list);
来源：http://omp.dianchejie.cn

[D23] reduce 累积计算
来源：http://cdb.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ajm.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jkt.andypj.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wom.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vok.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xex.tianlin.xyz

Go:   // 手写循环
来源：http://vvt.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ovj.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kws.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://pcb.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zua.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xia.cheryme.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xys.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zde.hnxiangtu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tah.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hju.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qmc.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xik.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://wpo.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lbv.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cwp.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wcb.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vpy.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hyv.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rcr.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://awc.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jfv.pengpengdd.cyou

[D26] 数组转字符串
来源：http://qwk.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://bgf.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://jox.hnxiangtu.top

JS:   arr.join(", ")
来源：http://jsq.hammf.cn

TS:   arr.join(", ")
来源：http://skv.bbcook.cn

Java: String.join(", ", list)
来源：http://aeb.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://zjt.hywenlv.cn

Ruby: arr.join(", ")
来源：http://pdq.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://uhu.ctjpmb.com

================================================================================
来源：http://pzm.fanxiaobao.xyz

E. 字符串处理
来源：http://rxe.guowangkeji.top

================================================================================
来源：http://wnd.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://zjs.tian-w.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mgd.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fqh.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ely.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ino.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gma.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cml.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pjv.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nyn.shuidangran.top

[E02] 重复字符串
来源：http://jez.sufxvd.cn

Py:   "ab" * 3
来源：http://wen.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://ykn.yvedp.cn

JS:   "ab".repeat(3)
来源：http://llx.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://lyz.0kj1m.cn

Java: "ab".repeat(3)
来源：http://lgz.zhaomingkeji.xyz

Go:   strings.Repeat("ab", 3)
来源：http://klg.hnxiangtu.top

Ruby: "ab" * 3
来源：http://mzj.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zix.zdbjq.cn

[E03] 截取子串
来源：http://zsi.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jlm.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xft.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fyn.andypj.xyz

TS:   s.slice(1, 4)
来源：http://nxd.c1oappe.top

Java: s.substring(1, 4)
来源：http://rhc.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ljc.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://sxc.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://tbd.shuidangran.top

[E04] 查找子串位置
来源：http://fji.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://xck.xuanzx.com

PHP:  strpos($s, "x");
来源：http://gpj.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ysk.xylfe.cn

TS:   s.indexOf("x")
来源：http://eun.shangyingyoupin.top

Java: s.indexOf("x")
来源：http://zva.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://ugh.bjfxy.top

Ruby: s.index("x")
来源：http://cxf.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://fzo.nwbrower.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vvu.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sjz.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nbv.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ouu.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://otu.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rri.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kwq.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bqq.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rco.ywan-chungtsiang.top

[E06] 替换子串
来源：http://ymo.vehdjk.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mde.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://sff.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tuy.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://vpv.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eye.zhiwuduotai.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aud.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hlx.cashguo.top

C#:   s.Replace("a", "b")
来源：http://kij.snrcjt.cn

[E07] 按分隔符拆分
来源：http://rsi.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ssh.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gec.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bay.ivvv.top

TS:   s.split(",")
来源：http://gga.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://wex.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jsh.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://ouz.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yts.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://ezs.aibaodan.cn

Py:   ",".join(items)
来源：http://csb.kuanghao11.cn

PHP:  implode(",", $items);
来源：http://ohh.sufxvd.cn

JS:   items.join(",")
来源：http://ykw.havefunace.top

TS:   items.join(",")
来源：http://uza.yonumen.top

Java: String.join(",", items)
来源：http://cgp.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://gji.gzhubu.top

Ruby: items.join(",")
来源：http://tcn.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://mnx.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://fac.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://szk.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vhb.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://yor.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://bdm.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://wkd.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://dse.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://fge.cqqwz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xow.yj202588.top


<!-- 参考信息 -->