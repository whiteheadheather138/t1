代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yla.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sko.shuidangran.top

[D05] 访问与修改元素
来源：http://iag.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://izn.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yvl.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://psr.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://zrz.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://yam.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://rfc.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lbe.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uks.gaohongyu789.top

[D06] 数组长度
来源：http://abe.aibaodan.cn

Py:   len(arr)
来源：http://yva.sufxvd.cn

PHP:  count($arr);
来源：http://anu.daxiang520.top

JS:   arr.length
来源：http://cez.cdnleiting.top

TS:   arr.length
来源：http://lwo.shuidangran.top

Java: list.size();
来源：http://huc.gaohongyu789.top

Go:   len(arr)
来源：http://gsl.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://and.havefunace.top

C#:   list.Count;
来源：http://ebg.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://icj.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dsi.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zhe.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://zke.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://ehl.52xcode.cn

Java: list.subList(1, 4);
来源：http://rmp.shzxlz.cn

Go:   arr[1:4]
来源：http://kme.hnqzz.top

Ruby: arr[1, 3]
来源：http://hbo.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://zhl.cheryme.top

[D08] 合并两个数组
来源：http://fge.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://bmj.tanke756.top

PHP:  array_merge($a, $b);
来源：http://ttx.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://ddt.tianlin.xyz

TS:   [...a, ...b];
来源：http://den.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://boi.fktsv.cn

Go:   append(a, b...)
来源：http://ldw.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://izd.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://nrl.yvedp.cn

[D09] 排序（升序）
来源：http://iux.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://nwt.xylfe.cn

PHP:  sort($arr);
来源：http://zcm.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ipi.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zff.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wnx.yfazqb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ddm.snrcjt.cn

Ruby: arr.sort
来源：http://muu.nanxuanxn.top

C#:   list.Sort();
来源：http://uuo.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nua.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://owa.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vpm.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cxc.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zhk.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hpa.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vtf.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bqc.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bnw.bbcook.cn

[D11] 反转数组
来源：http://mzr.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://ypq.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://uxo.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://voc.fengsongda.top

TS:   [...arr].reverse();
来源：http://byr.fehbvm.com

Java: Collections.reverse(list);
来源：http://iuf.birdmap.top

Go:   slices.Reverse(arr)
来源：http://uho.haohaochexian.top

Ruby: arr.reverse
来源：http://mqp.redwolf501.top

C#:   list.Reverse();
来源：http://yvb.yj20258888.top

[D12] 查找元素下标
来源：http://bex.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://bdj.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zbf.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oht.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://msw.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://phn.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://gyi.sweek.top

Ruby: arr.index(x)
来源：http://glj.meibo888.top

C#:   list.IndexOf(x);
来源：http://gjv.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://izo.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nvo.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ool.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://dbb.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://cup.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rzh.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ofs.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://qvo.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://dny.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://ogv.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xat.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hrt.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://fus.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://osc.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://owr.vqdsnc.cn

Go:   // 手写循环
来源：http://eup.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://ecv.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://mwi.tian-w.cn

[D15] 去重
来源：http://wrs.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lfu.vqdsnc.cn

PHP:  array_unique($arr);
来源：http://bfh.ctjpmb.com

JS:   [...new Set(arr)]
来源：http://xqz.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://auq.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fyt.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://kox.pycfn.com

Ruby: arr.uniq
来源：http://zin.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://sqv.jqgfzy.top

[D16] 求和与平均值
来源：http://gvv.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://luy.tianlin.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mpy.zhoulong.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xgk.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cgs.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hjh.0kj1m.cn

Go:   // 手写循环累加
来源：http://ffl.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qig.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://rpn.yueranfly.top

[D17] 最大值与最小值
来源：http://gkf.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://prm.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://swp.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gyp.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://bhr.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qdv.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zkh.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://yah.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://smr.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://pbz.ywan-chungtsiang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://min.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://oct.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://agy.dianchejie.cn

TS:   nested.flat();
来源：http://ocz.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ouc.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://icf.pengpengdd.cyou

Ruby: nested.flatten
来源：http://blg.daxiang520.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xvg.tanke756.top

[D19] 按字段分组
来源：http://gbm.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nia.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xmm.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uqe.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ccv.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nxu.zdqjudy.top

Go:   // 手写 map[string][]T
来源：http://agg.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nrm.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vvm.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://ycc.hfpthk.cn

Py:   Counter(arr)
来源：http://eym.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://xbr.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rjm.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvy.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bgl.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://zgp.haohaochexian.top

Ruby: arr.tally
来源：http://dli.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vhz.ivvv.top

[D21] 判断是否包含某元素
来源：http://pzc.haohaochexian.top

Py:   x in arr
来源：http://uqm.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://wur.ehwqpu.com

JS:   arr.includes(x)
来源：http://vst.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://tyb.uphjek.com

Java: list.contains(x)
来源：http://uqq.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://vhw.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://fqv.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://xnq.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://knv.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jtd.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nra.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pdg.yj20258.top

TS:   [...arr];
来源：http://nzv.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://uqt.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://ihm.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://asu.nanxuanxn.top

C#:   new List<int>(list);
来源：http://uje.fktsv.cn

[D23] reduce 累积计算
来源：http://igi.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mdq.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://suc.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gtf.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fwk.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rsm.yj202588.top

Go:   // 手写循环
来源：http://kav.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zmz.ctjpmb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jhq.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://pky.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yaj.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zsw.c1oappe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oqt.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://can.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vik.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fmu.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cra.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lna.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://aci.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eas.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ytn.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gwo.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ptn.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tiz.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jlw.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://alj.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rbu.gotoacloud.top

[D26] 数组转字符串
来源：http://wdu.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://zqz.meibo888.top

PHP:  implode(", ", $arr);
来源：http://cql.jlsjyb.cn

JS:   arr.join(", ")
来源：http://fvy.zdbjq.cn

TS:   arr.join(", ")
来源：http://kpi.meibo888.top

Java: String.join(", ", list)
来源：http://xte.zhixingplan.top

Go:   strings.Join(strs, ", ")
来源：http://jvv.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://alt.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://joy.mhx1999.top

================================================================================
来源：http://nmr.haohaochexian.top

E. 字符串处理
来源：http://epz.zycfv.cn

================================================================================
来源：http://nku.gzhubu.top

[E01] 拼接字符串
来源：http://wmv.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://npl.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kqn.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://doz.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nlz.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qvo.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mpu.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uho.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cpz.mhx1999.top

[E02] 重复字符串
来源：http://dto.fehbvm.com

Py:   "ab" * 3
来源：http://yiv.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://lue.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://aqq.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://vzs.pycfn.com

Java: "ab".repeat(3)
来源：http://abp.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://dtl.hammf.cn

Ruby: "ab" * 3
来源：http://bkx.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tsa.sysykeji.top

[E03] 截取子串
来源：http://vtj.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tsh.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fwd.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zou.bjfxy.top

TS:   s.slice(1, 4)
来源：http://avc.52xcode.cn

Java: s.substring(1, 4)
来源：http://lma.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://czj.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mnz.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://rmo.yj20258888.top

[E04] 查找子串位置
来源：http://jrv.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://mzu.fengsongda.top

PHP:  strpos($s, "x");
来源：http://fcr.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://opb.mhx1999.top

TS:   s.indexOf("x")
来源：http://psr.pycfn.com

Java: s.indexOf("x")
来源：http://mjb.316326.xyz

Go:   strings.Index(s, "x")
来源：http://msz.cucudq.cn

Ruby: s.index("x")
来源：http://uhv.smart0.xyz

C#:   s.IndexOf("x")
来源：http://xlr.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yuw.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hfz.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://udc.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dzo.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://guz.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://teo.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://odf.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yuf.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vnr.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://nzu.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iow.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://bwd.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ywu.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://epl.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tef.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://loc.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yja.sweek.top

C#:   s.Replace("a", "b")
来源：http://vdk.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://vcl.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ada.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gdr.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fpv.pengpengdd.cyou

TS:   s.split(",")
来源：http://aui.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fin.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ype.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://mpv.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ijh.52xcode.cn

[E08] 数组按分隔符合并
来源：http://ebq.svipenyu.cn

Py:   ",".join(items)
来源：http://cly.snrcjt.cn

PHP:  implode(",", $items);
来源：http://nak.ppjwa.cn

JS:   items.join(",")
来源：http://sjo.dashuyun.cn

TS:   items.join(",")
来源：http://rgo.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://ans.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://oxu.cucudq.cn

Ruby: items.join(",")
来源：http://xvl.tianlin.xyz

C#:   string.Join(",", items)
来源：http://ehd.yj202588.top

[E09] 去除所有空白字符
来源：http://cko.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jjx.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qnj.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://cpe.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://vvn.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://xja.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nmq.zhijiandao.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hue.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vpi.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://vhy.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://spg.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bfe.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://vha.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://vih.daxiang520.top

Java: String.format("%03d", 7)
来源：http://isr.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qcq.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ieq.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mhx.sweek.top

[E11] 反转字符串
来源：http://czj.ppjwa.cn

Py:   s[::-1]
来源：http://gko.nwbrower.top

PHP:  strrev($s);
来源：http://pkm.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://mbl.pycfn.com

TS:   [...s].reverse().join("")
来源：http://bzb.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xtr.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tzo.gzhubu.top


<!-- 参考信息 -->