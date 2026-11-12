代发 wailian999

Java: list.add(4);
来源：http://hgb.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://wfa.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://nwm.hysaishi.cn

C#:   list.Add(4);
来源：http://gww.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://hri.fehbvm.com

Py:   arr.insert(0, 0)
来源：http://bpa.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sxz.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zek.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://met.quarkkingdee.top

Java: list.add(0, 0);
来源：http://axl.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qcm.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xla.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://wsf.hnqzz.top

[D04] 删除元素
来源：http://nbs.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pmz.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mfy.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ihl.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://cci.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mqu.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://btf.shangyingyoupin.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ohs.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kmv.zhijiandao.cn

[D05] 访问与修改元素
来源：http://mir.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ozb.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cql.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://frw.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://yra.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://rvu.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://fau.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sfn.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wum.jinqigfzy.top

[D06] 数组长度
来源：http://kbu.gogol.net.cn

Py:   len(arr)
来源：http://jyp.havefunace.top

PHP:  count($arr);
来源：http://onx.quarkkingdee.top

JS:   arr.length
来源：http://qcd.gzhubu.top

TS:   arr.length
来源：http://bez.svipenyu.cn

Java: list.size();
来源：http://gsh.svipenyu.cn

Go:   len(arr)
来源：http://mfi.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://bsk.dianchejie.cn

C#:   list.Count;
来源：http://uqa.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://ozw.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hvl.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hig.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://djc.hammf.cn

TS:   arr.slice(1, 4);
来源：http://let.jqgfzy.top

Java: list.subList(1, 4);
来源：http://fkj.fengsongda.top

Go:   arr[1:4]
来源：http://cqr.jianghu66.top

Ruby: arr[1, 3]
来源：http://apf.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://mdj.nwbrower.top

[D08] 合并两个数组
来源：http://rju.birdmap.top

Py:   a + b;  a.extend(b)
来源：http://xhb.ehwqpu.com

PHP:  array_merge($a, $b);
来源：http://cao.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qgw.316326.xyz

TS:   [...a, ...b];
来源：http://rpg.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fdo.zdqjudy.top

Go:   append(a, b...)
来源：http://wci.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://yig.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://idk.pycfn.com

[D09] 排序（升序）
来源：http://fvp.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://pkl.smart0.xyz

PHP:  sort($arr);
来源：http://inf.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lre.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lci.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://brd.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jrc.hongshengwenyu.top

Ruby: arr.sort
来源：http://dwi.bjfxy.top

C#:   list.Sort();
来源：http://xsi.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hzt.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yak.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qjk.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qzs.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://led.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://onk.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gpy.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yis.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qzb.xuanzx.com

[D11] 反转数组
来源：http://jcd.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://kwm.jianghu66.top

PHP:  array_reverse($arr);
来源：http://tcs.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nwn.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://mbj.ppjwa.cn

Java: Collections.reverse(list);
来源：http://uvc.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://nhi.gogol.net.cn

Ruby: arr.reverse
来源：http://vpj.gotoacloud.top

C#:   list.Reverse();
来源：http://ehg.meibo888.top

[D12] 查找元素下标
来源：http://ahl.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://och.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fzu.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://utx.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zar.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kqb.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://cwz.zdqjudy.top

Ruby: arr.index(x)
来源：http://aas.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://phl.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://zpl.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pcy.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aro.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://lkn.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://hfi.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ycb.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jxv.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ljq.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hdr.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://nal.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://emj.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://php.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://esx.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://nbi.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://tql.andypj.xyz

Go:   // 手写循环
来源：http://xbc.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://yel.yj20258888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lwo.vqdsnc.cn

[D15] 去重
来源：http://ykj.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mny.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://sgx.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://lgt.yj20258888.top

TS:   [...new Set(arr)]
来源：http://atf.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dig.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://clh.dianchejie.cn

Ruby: arr.uniq
来源：http://fae.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://ire.zhixingplan.top

[D16] 求和与平均值
来源：http://qxu.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zbd.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qxs.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dzw.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uwj.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ukn.yvedp.cn

Go:   // 手写循环累加
来源：http://qze.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://atk.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://etq.zdqjudy.top

[D17] 最大值与最小值
来源：http://teb.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://ang.0kj1m.cn

PHP:  max($arr);  min($arr);
来源：http://mtw.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sli.ctjpmb.com

TS:   Math.max(...arr);
来源：http://oyb.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://msj.ivvv.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jom.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://hws.jiagoushi.top

C#:   list.Max();  list.Min()
来源：http://quy.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://uzm.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qsf.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://iml.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dmt.jiagoushi.top

TS:   nested.flat();
来源：http://xke.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yvd.bbcook.cn

Go:   // 手写双层循环
来源：http://hob.hnqzz.top

Ruby: nested.flatten
来源：http://fgm.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cox.xuanzx.com

[D19] 按字段分组
来源：http://jlt.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pvm.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xww.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://shj.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ehn.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ggu.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://ywj.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lbv.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lxj.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://kyv.wangshuangyany.cn

Py:   Counter(arr)
来源：http://doy.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://jgl.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qyx.bbcook.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fyc.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tav.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://wyw.ctjpmb.com

Ruby: arr.tally
来源：http://vnf.fktsv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zkq.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://lsn.zhiwuduotai.top

Py:   x in arr
来源：http://ufn.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://bki.guowangkeji.top

JS:   arr.includes(x)
来源：http://frg.jianghu66.top

TS:   arr.includes(x)
来源：http://eec.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://ywo.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://jtv.hysaishi.cn

Ruby: arr.include?(x)
来源：http://rsm.hnxiangtu.top

C#:   list.Contains(x)
来源：http://sju.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://hdz.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nst.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kff.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fag.zhongyouzk.top

TS:   [...arr];
来源：http://qfo.redwolf501.top

Java: new ArrayList<>(list);
来源：http://fgy.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://rdf.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://tos.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://vgm.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://eqv.shuidangran.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://siq.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uqe.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kpo.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aum.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tgp.0kj1m.cn

Go:   // 手写循环
来源：http://yfs.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kld.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rnt.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://ktk.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ofx.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pva.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://saf.daxiang520.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nbc.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tak.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sin.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eiq.cheryme.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zbr.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://ahc.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nnk.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nub.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://afp.vqdsnc.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dnq.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://odx.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://slj.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qhl.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wxz.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://kny.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://vsl.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://vlf.cdnleiting.top

JS:   arr.join(", ")
来源：http://alf.zhoulong.xyz

TS:   arr.join(", ")
来源：http://cuo.cucudq.cn

Java: String.join(", ", list)
来源：http://nro.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://nrs.shzxlz.cn

Ruby: arr.join(", ")
来源：http://kgl.mhx1999.top

C#:   string.Join(", ", list)
来源：http://bpp.gzhubu.top

================================================================================
来源：http://pty.xylfe.cn

E. 字符串处理
来源：http://fnb.shangyingyoupin.top

================================================================================
来源：http://yaf.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://wfg.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wxa.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jij.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qhp.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qxq.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://npt.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uhp.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jjj.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kal.0kj1m.cn

[E02] 重复字符串
来源：http://cme.9152youxi.cn

Py:   "ab" * 3
来源：http://lxc.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://bnb.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://fyb.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://cma.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://vcy.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://vcy.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://fxx.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iek.wangshuangyany.cn

[E03] 截取子串
来源：http://gnd.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ujj.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://urc.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lhl.yueranfly.top

TS:   s.slice(1, 4)
来源：http://orb.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://zzb.fanxiaobao.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zib.hywenlv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kmv.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://wur.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://ete.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://dvx.daxiang520.top

PHP:  strpos($s, "x");
来源：http://zyn.zycfv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uzw.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://uah.zycfv.cn

Java: s.indexOf("x")
来源：http://cbp.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://ohd.xinyue.icu

Ruby: s.index("x")
来源：http://gwd.fengsongda.top

C#:   s.IndexOf("x")
来源：http://lkt.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://plp.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bas.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mhm.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xcp.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uob.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eeh.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://myp.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dmb.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nzu.yj20258888.top

[E06] 替换子串
来源：http://pgy.guannengcc.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ecz.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://rwu.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bbw.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://uvj.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://del.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wrg.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eub.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://inl.ehwqpu.com

[E07] 按分隔符拆分
来源：http://kmx.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wku.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nqv.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://szk.daria6918.cn

TS:   s.split(",")
来源：http://hwy.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://fao.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sre.yongpay.top

Ruby: s.split(",");  s.split
来源：http://rne.jlsjyb.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mst.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://ubc.ydjk.org.cn

Py:   ",".join(items)
来源：http://wah.xylfe.cn

PHP:  implode(",", $items);
来源：http://dwp.tianlin.xyz

JS:   items.join(",")
来源：http://fpm.chenzaomai.com

TS:   items.join(",")
来源：http://kop.wangshuangyany.cn

Java: String.join(",", items)
来源：http://dag.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://ppr.ehwqpu.com

Ruby: items.join(",")
来源：http://ibw.yfazqb.com

C#:   string.Join(",", items)
来源：http://gqb.daria6918.cn

[E09] 去除所有空白字符
来源：http://gto.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xdh.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oss.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://cph.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://rrw.tanke756.top


<!-- 参考信息 -->