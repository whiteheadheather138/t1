代发 wailian999

C#:   list.Insert(0, 0);
来源：http://fsf.gzhubu.top

[D04] 删除元素
来源：http://nyg.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://krq.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://utg.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ygf.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://fib.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uks.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qom.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iyy.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wys.cqqwz.cn

[D05] 访问与修改元素
来源：http://ksr.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aki.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zod.shzxlz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nxq.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://dml.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://piq.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://zya.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://stb.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eix.zdqjudy.top

[D06] 数组长度
来源：http://tnn.zhijiandao.cn

Py:   len(arr)
来源：http://qxb.guannengcc.top

PHP:  count($arr);
来源：http://icw.yonumen.top

JS:   arr.length
来源：http://qdd.gotoacloud.top

TS:   arr.length
来源：http://kue.kuanghao11.cn

Java: list.size();
来源：http://kof.shuidangran.top

Go:   len(arr)
来源：http://zzz.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://opd.bjfxy.top

C#:   list.Count;
来源：http://wrk.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://hcq.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://azm.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fel.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://awj.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://zed.wangdashe.top

Java: list.subList(1, 4);
来源：http://qiu.sysykeji.top

Go:   arr[1:4]
来源：http://val.aibaodan.cn

Ruby: arr[1, 3]
来源：http://ifc.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://gth.uphjek.com

[D08] 合并两个数组
来源：http://tvt.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://nxj.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://nji.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fea.yj202588.top

TS:   [...a, ...b];
来源：http://ill.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://med.chenlongwang.top

Go:   append(a, b...)
来源：http://ibs.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://toy.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://utn.bjfxy.top

[D09] 排序（升序）
来源：http://bzk.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://mwj.snrcjt.cn

PHP:  sort($arr);
来源：http://dmg.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ozh.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mch.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qlg.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lit.sxryk.cn

Ruby: arr.sort
来源：http://zqe.aizwys.cn

C#:   list.Sort();
来源：http://oqq.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dry.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wbx.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yzu.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fqr.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zsw.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nef.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qnq.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ubf.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dzg.chenlongwang.top

[D11] 反转数组
来源：http://atn.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://bvl.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://qwz.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xpm.cashguo.top

TS:   [...arr].reverse();
来源：http://dtd.chenlongwang.top

Java: Collections.reverse(list);
来源：http://yxn.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://del.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://ryd.shangyingyoupin.top

C#:   list.Reverse();
来源：http://zdg.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://rxi.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://bvz.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vvi.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrs.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ums.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hjf.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://tnw.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://vpp.cashguo.top

C#:   list.IndexOf(x);
来源：http://qnb.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://ykv.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lkj.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://epc.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://hnh.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://gsc.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ztq.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qgu.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ddm.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vlp.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://arn.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ivt.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://goc.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://ubd.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://xgh.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://efk.bjfxy.top

Go:   // 手写循环
来源：http://llc.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://rzv.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wtt.yuanzhike.top

[D15] 去重
来源：http://dar.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qrt.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://vsl.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://rqt.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://vwk.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cpn.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://rdk.svipenyu.cn

Ruby: arr.uniq
来源：http://yyq.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://wvm.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://jew.aizwys.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zty.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pau.0kj1m.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cpp.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qlr.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yyt.nanxinkj.top

Go:   // 手写循环累加
来源：http://ddk.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kic.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://kkz.ehwqpu.com

[D17] 最大值与最小值
来源：http://zzd.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://msx.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://kpu.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gri.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://kjb.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nrz.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mpt.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://ddb.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://nwr.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://hpm.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mqi.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://gll.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cbd.chenzaomai.com

TS:   nested.flat();
来源：http://iyx.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lmo.vqdsnc.cn

Go:   // 手写双层循环
来源：http://uxz.52xcode.cn

Ruby: nested.flatten
来源：http://vwk.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sus.shangyingyoupin.top

[D19] 按字段分组
来源：http://erb.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rro.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nnv.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iwi.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hrm.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://abq.yj202588.top

Go:   // 手写 map[string][]T
来源：http://wdq.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ipb.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ahx.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://bfw.jinqigfzy.top

Py:   Counter(arr)
来源：http://zrl.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://cmy.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qym.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jyk.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qxp.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://zws.gaohongyu789.top

Ruby: arr.tally
来源：http://jex.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kgm.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://xka.zhengqikj.top

Py:   x in arr
来源：http://rbm.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://xpi.gzhubu.top

JS:   arr.includes(x)
来源：http://msn.vqdsnc.cn

TS:   arr.includes(x)
来源：http://lgj.yanxiufei.cn

Java: list.contains(x)
来源：http://gzr.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://qsw.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://mlf.zhijiandao.cn

C#:   list.Contains(x)
来源：http://zxb.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://ggv.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hly.fanxiaobao.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rgm.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qbd.haohaochexian.top

TS:   [...arr];
来源：http://xqb.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://eap.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://pua.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://lpt.fehbvm.com

C#:   new List<int>(list);
来源：http://lqg.yj202588.top

[D23] reduce 累积计算
来源：http://gar.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://voc.zycfv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bzk.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bqv.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lry.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tuj.gotoacloud.top

Go:   // 手写循环
来源：http://iek.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://omc.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zxt.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://eyh.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://usm.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hot.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wli.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hnt.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hob.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qnw.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://piu.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ecw.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://qqb.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ojo.xuetiantiany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://emq.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://esa.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vse.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ooc.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dww.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oxa.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uhw.shzxlz.cn

[D26] 数组转字符串
来源：http://php.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://nud.tarul.cn

PHP:  implode(", ", $arr);
来源：http://bme.nwbrower.top

JS:   arr.join(", ")
来源：http://jjz.nanxinkj.top

TS:   arr.join(", ")
来源：http://syz.ydzc1.top

Java: String.join(", ", list)
来源：http://jai.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://nqe.gzhubu.top

Ruby: arr.join(", ")
来源：http://bqj.sysykeji.top

C#:   string.Join(", ", list)
来源：http://xqp.zhaomingkeji.xyz

================================================================================
来源：http://eoh.cqqwz.cn

E. 字符串处理
来源：http://pzv.tanke756.top

================================================================================
来源：http://ovy.zhijiandao.cn

[E01] 拼接字符串
来源：http://rwt.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zzf.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gax.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kwm.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wwt.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ohs.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fdc.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hbm.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kyx.sxryk.cn

[E02] 重复字符串
来源：http://xyx.fktsv.cn

Py:   "ab" * 3
来源：http://qer.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://fvn.316326.xyz

JS:   "ab".repeat(3)
来源：http://iun.ivvv.top

TS:   "ab".repeat(3)
来源：http://njn.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://hsx.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://afw.jqgufenzy.top

Ruby: "ab" * 3
来源：http://qbu.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://udt.hcnkem.com

[E03] 截取子串
来源：http://zjh.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zlj.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xsw.yj20258888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yof.yj20258888.top

TS:   s.slice(1, 4)
来源：http://qhs.daria6918.cn

Java: s.substring(1, 4)
来源：http://uis.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://esj.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://hhx.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://pkk.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://jdj.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://geg.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://wsj.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://whd.gogol.net.cn

TS:   s.indexOf("x")
来源：http://efv.zhengqikj.top

Java: s.indexOf("x")
来源：http://adj.jqgfzy.top

Go:   strings.Index(s, "x")
来源：http://xer.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://suo.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://ong.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://orx.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fhx.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mde.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bbf.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://amm.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ohf.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zdn.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://giy.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oex.ywan-chungtsiang.top

[E06] 替换子串
来源：http://epp.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://irs.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://uam.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iun.dashuyun.cn

TS:   s.replaceAll("a", "b")
来源：http://jbu.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vnr.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://scy.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://odp.hammf.cn

C#:   s.Replace("a", "b")
来源：http://iqp.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://xiy.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xuo.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hdy.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pcf.hongshengwenyu.top

TS:   s.split(",")
来源：http://zue.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://xdi.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jkv.kuanghao11.cn

Ruby: s.split(",");  s.split
来源：http://aaz.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bra.jlsjyb.cn

[E08] 数组按分隔符合并
来源：http://ntg.jqgufenzy.top

Py:   ",".join(items)
来源：http://hqk.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://msc.yangfankeji.com

JS:   items.join(",")
来源：http://ayt.shanyushiyangtech.top

TS:   items.join(",")
来源：http://rav.jinqigfzy.top

Java: String.join(",", items)
来源：http://jwb.aibaodan.cn

Go:   strings.Join(items, ",")
来源：http://rpx.xziqi.cn

Ruby: items.join(",")
来源：http://oiw.uphjek.com

C#:   string.Join(",", items)
来源：http://qch.iojbl.cn

[E09] 去除所有空白字符
来源：http://erg.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mjb.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lbx.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://gii.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://akc.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://fhz.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://xyh.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://vds.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ucz.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://hti.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xpn.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fms.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://xdn.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://cga.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://qry.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://iur.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://feo.nanxinkj.top


<!-- 参考信息 -->