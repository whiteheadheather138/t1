代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zfn.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pad.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fvq.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gpt.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://sdk.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://ozk.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rqb.ydzc1.top

[D02] 追加元素到末尾
来源：http://umo.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mre.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tsa.gogol.net.cn

JS:   arr.push(4);
来源：http://qmx.jqgfzy.top

TS:   arr.push(4);
来源：http://oqn.fktsv.cn

Java: list.add(4);
来源：http://bwb.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://ifq.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://ecf.hfpthk.cn

C#:   list.Add(4);
来源：http://jpz.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://oeh.yongpay.top

Py:   arr.insert(0, 0)
来源：http://wem.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aog.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ndk.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://bdj.gaohongyu789.top

Java: list.add(0, 0);
来源：http://dti.sysykeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://mcd.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fah.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://fmf.xziqi.cn

[D04] 删除元素
来源：http://avi.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pcb.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vja.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lxl.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://qry.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://abh.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bpi.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://smv.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hbj.pycfn.com

[D05] 访问与修改元素
来源：http://lgq.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xbc.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bpw.aibaodan.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fhs.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://iwa.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://chq.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://wzn.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://slv.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kzs.zhixingplan.top

[D06] 数组长度
来源：http://kvb.jinghuilouyu.cn

Py:   len(arr)
来源：http://vpn.52xcode.cn

PHP:  count($arr);
来源：http://ruq.ybcxt.top

JS:   arr.length
来源：http://eal.sysykeji.top

TS:   arr.length
来源：http://thh.uphjek.com

Java: list.size();
来源：http://hmr.smart0.xyz

Go:   len(arr)
来源：http://bof.zycfv.cn

Ruby: arr.length; arr.size
来源：http://mhb.hfpthk.cn

C#:   list.Count;
来源：http://lpj.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://acb.sjlbkw.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sss.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://jno.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://gvv.cheryme.top

TS:   arr.slice(1, 4);
来源：http://yhv.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://tcj.snrcjt.cn

Go:   arr[1:4]
来源：http://ksh.xinyue.icu

Ruby: arr[1, 3]
来源：http://clu.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://uzm.yanxiufei.cn

[D08] 合并两个数组
来源：http://cwv.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://snd.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://qyr.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cwb.9152youxi.cn

TS:   [...a, ...b];
来源：http://dkf.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kkv.yuxming.cn

Go:   append(a, b...)
来源：http://wyv.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://mkd.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://mwh.epnwcf.com

[D09] 排序（升序）
来源：http://gbp.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://fbi.gzhubu.top

PHP:  sort($arr);
来源：http://ibi.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://crj.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://aax.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nmz.zdbjq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pac.yj202588.top

Ruby: arr.sort
来源：http://mfg.guowangkeji.top

C#:   list.Sort();
来源：http://fep.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pwb.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mpl.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kzk.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://buo.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bqq.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cot.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mze.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uba.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://let.hnqzz.top

[D11] 反转数组
来源：http://ukh.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://pgz.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://zol.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ina.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://wtn.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://gky.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://nkm.52xcode.cn

Ruby: arr.reverse
来源：http://xrd.hnxiangtu.top

C#:   list.Reverse();
来源：http://iwb.ppjwa.cn

[D12] 查找元素下标
来源：http://eif.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://pdg.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zpm.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jui.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bms.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://erh.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://mpb.mhx1999.top

Ruby: arr.index(x)
来源：http://lls.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://wsx.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://idi.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gtd.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ibe.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://kka.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://yxf.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cei.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qiq.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://smg.sjlbkw.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://doh.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://waz.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dly.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hiw.xylfe.cn

JS:   arr.map(x => x * 2)
来源：http://fmc.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://mfd.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://niw.hongshengwenyu.top

Go:   // 手写循环
来源：http://wzf.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://huk.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yzb.wangdashe.top

[D15] 去重
来源：http://kdq.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xmy.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://usf.sweek.top

JS:   [...new Set(arr)]
来源：http://wuq.cheryme.top

TS:   [...new Set(arr)]
来源：http://eea.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uxx.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://tai.daria6918.cn

Ruby: arr.uniq
来源：http://mri.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://vfj.shangyingyoupin.top

[D16] 求和与平均值
来源：http://dxm.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xqu.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rxh.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rsn.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pol.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://quw.ctjpmb.com

Go:   // 手写循环累加
来源：http://muh.smart0.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qbt.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://nsz.epnwcf.com

[D17] 最大值与最小值
来源：http://jpw.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://jza.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://lyh.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zuk.ehwqpu.com

TS:   Math.max(...arr);
来源：http://yzw.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gej.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ygc.sweek.top

Ruby: arr.max;  arr.min
来源：http://sjz.dianchejie.cn

C#:   list.Max();  list.Min()
来源：http://xmf.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://rhm.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdy.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://cwx.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sln.sufxvd.cn

TS:   nested.flat();
来源：http://vuq.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ggi.daxiang520.top

Go:   // 手写双层循环
来源：http://wgk.zycfv.cn

Ruby: nested.flatten
来源：http://tbg.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://bdh.mhx1999.top

[D19] 按字段分组
来源：http://iqq.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rqh.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://czt.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iwl.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://iuj.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://txh.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://jxv.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vhn.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hxf.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://xcq.xinyue.icu

Py:   Counter(arr)
来源：http://afc.fktsv.cn

PHP:  array_count_values($arr);
来源：http://moz.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cmy.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://amf.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uci.ybcxt.top

Go:   // 手写 map[T]int
来源：http://qoq.dashuyun.cn

Ruby: arr.tally
来源：http://rnq.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wpc.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://dci.fengsongda.top

Py:   x in arr
来源：http://iwu.kuanghao11.cn

PHP:  in_array($x, $arr, true);
来源：http://kdo.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://wuy.pycfn.com

TS:   arr.includes(x)
来源：http://aqp.ehwqpu.com

Java: list.contains(x)
来源：http://spc.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://yao.yj20258888.top

Ruby: arr.include?(x)
来源：http://zek.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://voj.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://blw.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ixz.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vhl.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://odf.iojbl.cn

TS:   [...arr];
来源：http://ixj.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://czf.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://pym.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://xmp.chenzaomai.com

C#:   new List<int>(list);
来源：http://ruo.vqdsnc.cn

[D23] reduce 累积计算
来源：http://hiu.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zdb.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vwi.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pws.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kht.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kvr.zhongyouzk.top

Go:   // 手写循环
来源：http://qvs.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ciz.guannengcc.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rio.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://qmw.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zsa.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ovw.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gzn.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ctv.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://unu.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ild.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cok.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vmc.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://wzj.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gjh.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dtz.yvedp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bgn.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gwr.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wmx.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rom.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://czh.aibaodan.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aqx.iojbl.cn

[D26] 数组转字符串
来源：http://tkp.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://yeh.ivvv.top

PHP:  implode(", ", $arr);
来源：http://tpk.hysaishi.cn

JS:   arr.join(", ")
来源：http://poz.redwolf501.top

TS:   arr.join(", ")
来源：http://oiy.ydjk.org.cn

Java: String.join(", ", list)
来源：http://cve.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://drr.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://bxf.havefunace.top

C#:   string.Join(", ", list)
来源：http://xyu.yongpay.top

================================================================================
来源：http://vwl.ctjpmb.com

E. 字符串处理
来源：http://ipn.shanyushiyangkeji.top

================================================================================
来源：http://dsj.iojbl.cn

[E01] 拼接字符串
来源：http://vrf.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lof.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qmb.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://abm.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://per.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://shr.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bxe.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rkh.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wzj.xuanzx.com

[E02] 重复字符串
来源：http://yoy.smart0.xyz

Py:   "ab" * 3
来源：http://khs.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://itq.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://fgt.ydzc1.top

TS:   "ab".repeat(3)
来源：http://syb.fengsongda.top

Java: "ab".repeat(3)
来源：http://swb.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://jqe.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://kvx.chenjidiqi.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vuh.hammf.cn

[E03] 截取子串
来源：http://koc.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kfs.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rmj.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://acq.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://svn.jiagoushi.top

Java: s.substring(1, 4)
来源：http://obv.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qjx.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://bxq.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://nob.quarkkingdee.top

[E04] 查找子串位置
来源：http://gdz.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://lio.bjfxy.top

PHP:  strpos($s, "x");
来源：http://dvy.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fut.gzhubu.top

TS:   s.indexOf("x")
来源：http://fln.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://nla.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://iug.ivvv.top

Ruby: s.index("x")
来源：http://yup.tanke756.top

C#:   s.IndexOf("x")
来源：http://egp.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://cie.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hvg.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ofi.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ahg.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sze.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nmo.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lok.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cgj.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rln.ctjpmb.com

[E06] 替换子串
来源：http://sth.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vsi.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://gfc.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kpq.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://rwp.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ail.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vdw.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bmw.pycfn.com

C#:   s.Replace("a", "b")
来源：http://bnp.xinyue.icu

[E07] 按分隔符拆分
来源：http://bfb.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tfn.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vxh.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://krr.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://yso.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://kpd.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kue.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://dxp.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eyl.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://pya.fzhhl.top

Py:   ",".join(items)
来源：http://rwb.ydzc1.top


<!-- 参考信息 -->