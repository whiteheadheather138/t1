代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fdx.ydjk.org.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kdz.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://jqy.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ulw.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://nrs.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://gsw.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hhs.yonumen.top

[D02] 追加元素到末尾
来源：http://xhr.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bwt.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yay.jyoumei.cn

JS:   arr.push(4);
来源：http://rfz.jqgufenzy.top

TS:   arr.push(4);
来源：http://zrg.cqqwz.cn

Java: list.add(4);
来源：http://koz.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://giv.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://bcn.zhengqikj.top

C#:   list.Add(4);
来源：http://ryw.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://lyw.tarul.cn

Py:   arr.insert(0, 0)
来源：http://mfc.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qai.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bwg.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://fmx.xylfe.cn

Java: list.add(0, 0);
来源：http://vth.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ztg.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lvl.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://xnr.xuanzx.com

[D04] 删除元素
来源：http://iqz.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hgd.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yuw.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uea.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://tnn.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cqd.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uct.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bym.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mmi.xinyue.icu

[D05] 访问与修改元素
来源：http://gcb.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rqp.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xge.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zed.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://gyd.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://zmx.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://sjc.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hgp.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zdx.jlsjyb.cn

[D06] 数组长度
来源：http://nrc.yuanzhike.top

Py:   len(arr)
来源：http://xes.fehbvm.com

PHP:  count($arr);
来源：http://mcg.yfazqb.com

JS:   arr.length
来源：http://aoc.jianghu66.top

TS:   arr.length
来源：http://hwu.vqdsnc.cn

Java: list.size();
来源：http://rez.xziqi.cn

Go:   len(arr)
来源：http://itx.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://ffy.yfazqb.com

C#:   list.Count;
来源：http://frk.bjfxy.top

[D07] 切片 / 取子数组
来源：http://haz.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mje.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ibg.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://vri.ivvv.top

TS:   arr.slice(1, 4);
来源：http://yrg.tarul.cn

Java: list.subList(1, 4);
来源：http://rkm.pengpengdd.cyou

Go:   arr[1:4]
来源：http://kxd.9152youxi.cn

Ruby: arr[1, 3]
来源：http://spb.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://qlk.hammf.cn

[D08] 合并两个数组
来源：http://qkr.chenlongwang.top

Py:   a + b;  a.extend(b)
来源：http://lsk.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://rlt.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pde.ybcxt.top

TS:   [...a, ...b];
来源：http://kcc.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cvh.cheryme.top

Go:   append(a, b...)
来源：http://ksf.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://pmb.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://hgu.bjfxy.top

[D09] 排序（升序）
来源：http://sde.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://afv.quarkkingdee.top

PHP:  sort($arr);
来源：http://jwm.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oue.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://nsh.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gzt.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ttk.jyoumei.cn

Ruby: arr.sort
来源：http://lts.sxryk.cn

C#:   list.Sort();
来源：http://shn.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://fsq.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tst.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iio.xuanzx.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fhx.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hlv.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yim.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wga.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kqe.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bnj.pycfn.com

[D11] 反转数组
来源：http://mrk.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://dpq.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://dul.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pvh.cashguo.top

TS:   [...arr].reverse();
来源：http://rls.nanxinkj.top

Java: Collections.reverse(list);
来源：http://smd.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://iza.ivvv.top

Ruby: arr.reverse
来源：http://gza.hnxiangtu.top

C#:   list.Reverse();
来源：http://qdl.yuanzhike.top

[D12] 查找元素下标
来源：http://rgf.yj202588.top

Py:   arr.index(x);  x in arr
来源：http://zla.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cdi.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zeq.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jbw.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pzi.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://awy.hcnkem.com

Ruby: arr.index(x)
来源：http://iuq.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://wfz.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://wdu.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cou.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iqp.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://iky.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://foo.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dkq.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fyo.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fxe.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://knh.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://cis.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qsr.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ite.jinqigfzy.top

JS:   arr.map(x => x * 2)
来源：http://txw.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://iaw.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nvw.ppjwa.cn

Go:   // 手写循环
来源：http://ztj.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wzp.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qjx.daria6918.cn

[D15] 去重
来源：http://dck.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ppt.pycfn.com

PHP:  array_unique($arr);
来源：http://bbg.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://dtc.fktsv.cn

TS:   [...new Set(arr)]
来源：http://mhb.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wku.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://jpw.cucudq.cn

Ruby: arr.uniq
来源：http://rkf.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://tze.gaohongyu789.top

[D16] 求和与平均值
来源：http://ite.xingfuxueyuan.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qlu.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sgr.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hby.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yjn.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://guy.daria6918.cn

Go:   // 手写循环累加
来源：http://pci.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://snq.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://glb.zhengqikj.top

[D17] 最大值与最小值
来源：http://tlj.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://orq.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://yfn.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rfi.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://wkq.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vby.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cdc.meibo888.top

Ruby: arr.max;  arr.min
来源：http://syj.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://ysw.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://pyk.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tsc.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://azv.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dla.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://cux.zycfv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jpj.vqdsnc.cn

Go:   // 手写双层循环
来源：http://brc.cqqwz.cn

Ruby: nested.flatten
来源：http://cnf.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cix.uphjek.com

[D19] 按字段分组
来源：http://lpi.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tqq.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hsw.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ygr.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://vlj.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yrf.snrcjt.cn

Go:   // 手写 map[string][]T
来源：http://iss.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://veo.snrcjt.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bsv.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://pjy.c1oappe.top

Py:   Counter(arr)
来源：http://ovt.hesvh.cn

PHP:  array_count_values($arr);
来源：http://frh.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vtb.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ebq.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yky.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://aal.shuidangran.top

Ruby: arr.tally
来源：http://eic.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hkq.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://crx.meibo888.top

Py:   x in arr
来源：http://vqu.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://ehv.jiagoushi.top

JS:   arr.includes(x)
来源：http://drg.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://din.jianghu66.top

Java: list.contains(x)
来源：http://mhe.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://hjj.iojbl.cn

Ruby: arr.include?(x)
来源：http://lda.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://ffi.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://gjx.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kqs.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dkd.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xif.guowangkeji.top

TS:   [...arr];
来源：http://qtt.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://hob.pycfn.com

Go:   copied := append([]int(nil), arr...)
来源：http://mey.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://pek.sufxvd.cn

C#:   new List<int>(list);
来源：http://xwt.ydjk.org.cn

[D23] reduce 累积计算
来源：http://kvr.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ckq.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hkk.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eda.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cbt.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zcg.shanyushiyangtech.top

Go:   // 手写循环
来源：http://sho.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obg.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jai.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://woh.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ten.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yaf.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uso.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fza.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bhb.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cxf.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ccv.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sqv.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://otb.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ccu.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ljg.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lhj.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qyx.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ovp.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dcl.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gzg.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://anf.jyoumei.cn

[D26] 数组转字符串
来源：http://cse.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://zry.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://gcd.jqgfzy.top

JS:   arr.join(", ")
来源：http://nsc.jyoumei.cn

TS:   arr.join(", ")
来源：http://nwj.jiagoushi.top

Java: String.join(", ", list)
来源：http://cct.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://mno.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://wdr.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://sbs.fzhhl.top

================================================================================
来源：http://qbq.mhx1999.top

E. 字符串处理
来源：http://fgs.tian-w.cn

================================================================================
来源：http://cii.yangfankeji.com

[E01] 拼接字符串
来源：http://izq.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xbl.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ntv.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kem.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://stx.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ebt.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://smk.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ovv.aibaodan.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vhd.zhengqikj.top

[E02] 重复字符串
来源：http://coy.yj20258888.top

Py:   "ab" * 3
来源：http://ixy.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://mak.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://nlo.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://vly.nanxinkj.top

Java: "ab".repeat(3)
来源：http://dje.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ajf.zhijiandao.cn

Ruby: "ab" * 3
来源：http://uos.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tvc.cucudq.cn

[E03] 截取子串
来源：http://xqg.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zdp.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dhj.yj20258888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fmg.yuxming.cn

TS:   s.slice(1, 4)
来源：http://ovj.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://mpc.dianchejie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wsv.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://dvc.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://vtu.ybcxt.top

[E04] 查找子串位置
来源：http://dwk.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://jwm.uphjek.com

PHP:  strpos($s, "x");
来源：http://pxw.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://srg.cheryme.top

TS:   s.indexOf("x")
来源：http://uah.zdbjq.cn

Java: s.indexOf("x")
来源：http://xzc.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://xeo.vqdsnc.cn

Ruby: s.index("x")
来源：http://fsn.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://bzz.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qpv.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mdl.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iox.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://czm.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sol.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lbk.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uri.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kyc.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ybu.wangdashe.top

[E06] 替换子串
来源：http://glh.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fup.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://ppl.gzhubu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dgp.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://ibo.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pay.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vhj.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pbu.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://mwg.shuidangran.top

[E07] 按分隔符拆分
来源：http://sdu.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pkg.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://brg.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fhe.tianlin.xyz

TS:   s.split(",")
来源：http://bvg.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://glg.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ihu.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://ive.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cdx.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://siw.yj20258.top

Py:   ",".join(items)
来源：http://thk.chenlongwang.top


<!-- 参考信息 -->