代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kka.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ssn.dianchejie.cn

JS:   arr.push(4);
来源：http://nng.tanke756.top

TS:   arr.push(4);
来源：http://oud.zhijiandao.cn

Java: list.add(4);
来源：http://qvg.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://uku.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://luj.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://flt.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://wzi.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://ypu.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bcr.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aey.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://gfj.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://ila.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://lsw.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zgj.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://bgp.fktsv.cn

[D04] 删除元素
来源：http://hgj.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xle.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eeg.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kfp.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://and.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pet.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ncv.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nou.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xvj.zhijiandao.cn

[D05] 访问与修改元素
来源：http://ldn.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aih.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vqr.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zfw.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://twg.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://apw.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://tdc.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wes.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://erl.jinqigufen.top

[D06] 数组长度
来源：http://tib.hfpthk.cn

Py:   len(arr)
来源：http://ypx.hongshengwenyu.top

PHP:  count($arr);
来源：http://zrc.xinyue.icu

JS:   arr.length
来源：http://hxd.tian-w.cn

TS:   arr.length
来源：http://fqk.zhoulong.xyz

Java: list.size();
来源：http://rjb.yj20258888.top

Go:   len(arr)
来源：http://upz.yvedp.cn

Ruby: arr.length; arr.size
来源：http://opj.pengpengdd.cyou

C#:   list.Count;
来源：http://rwq.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://drh.jinghuilouyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xnq.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://sst.guowangkeji.top

JS:   arr.slice(1, 4);
来源：http://eml.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://cau.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://qls.nwbrower.top

Go:   arr[1:4]
来源：http://qsf.cqqwz.cn

Ruby: arr[1, 3]
来源：http://dvr.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://itu.zhiwuduotai.top

[D08] 合并两个数组
来源：http://uja.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://zvv.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://cxi.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lpm.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://jcs.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dxs.zhijiandao.cn

Go:   append(a, b...)
来源：http://kts.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://rul.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://uhx.yj202588.top

[D09] 排序（升序）
来源：http://nod.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://bwo.feifeiyinyue.top

PHP:  sort($arr);
来源：http://han.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bzc.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://kri.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dhd.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://exv.jqgfzy.top

Ruby: arr.sort
来源：http://ekw.guannengcc.top

C#:   list.Sort();
来源：http://ppl.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tqv.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vhm.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://joi.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oln.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pma.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://idm.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ros.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wmh.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hut.yj202588.top

[D11] 反转数组
来源：http://jcm.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://vcz.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://pwj.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mev.chenzaomai.com

TS:   [...arr].reverse();
来源：http://hna.ehwqpu.com

Java: Collections.reverse(list);
来源：http://yhh.jianghu66.top

Go:   slices.Reverse(arr)
来源：http://vrp.tarul.cn

Ruby: arr.reverse
来源：http://dil.daria6918.cn

C#:   list.Reverse();
来源：http://cyr.jqgufenzy.top

[D12] 查找元素下标
来源：http://gbw.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://ist.ydzc1.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nxq.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qcc.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gqi.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://suz.guowangkeji.top

Go:   slices.Index(arr, x)
来源：http://ohg.sufxvd.cn

Ruby: arr.index(x)
来源：http://iui.yongpay.top

C#:   list.IndexOf(x);
来源：http://ljg.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://mgi.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lkn.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ohc.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://crv.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://nsa.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://avb.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rby.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://tkr.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ljo.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://wvh.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tns.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://esb.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://rzt.9152youxi.cn

TS:   arr.map(x => x * 2)
来源：http://eao.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jtc.tianlin.xyz

Go:   // 手写循环
来源：http://gsq.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://uvq.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://yjb.jinqigufen.top

[D15] 去重
来源：http://iim.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://paa.ybcxt.top

PHP:  array_unique($arr);
来源：http://zwp.uphjek.com

JS:   [...new Set(arr)]
来源：http://yof.jianghu66.top

TS:   [...new Set(arr)]
来源：http://ldc.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yvo.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://emy.9152youxi.cn

Ruby: arr.uniq
来源：http://ipp.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://abg.wangdashe.top

[D16] 求和与平均值
来源：http://tmf.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mcx.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pqg.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://phc.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vih.zdbjq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bkz.jqgufenzy.top

Go:   // 手写循环累加
来源：http://rro.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://omu.daxiang520.top

C#:   list.Sum();  list.Average()
来源：http://nzk.hesvh.cn

[D17] 最大值与最小值
来源：http://aol.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://nph.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://rju.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wmv.yuanzhike.top

TS:   Math.max(...arr);
来源：http://zfi.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wyq.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wuy.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://qvm.cdnleiting.top

C#:   list.Max();  list.Min()
来源：http://kdu.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://xfk.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vqj.zhixingplan.top

PHP:  array_merge(...$nested);
来源：http://uzt.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bus.yueranfly.top

TS:   nested.flat();
来源：http://htv.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://diw.bjfxy.top

Go:   // 手写双层循环
来源：http://cwe.mhx1999.top

Ruby: nested.flatten
来源：http://zgt.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ney.vehdjk.com

[D19] 按字段分组
来源：http://eoy.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ebk.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://brj.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wzc.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ozg.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://trz.yongpay.top

Go:   // 手写 map[string][]T
来源：http://dip.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://twr.shanyushiyangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qie.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://veh.nwbrower.top

Py:   Counter(arr)
来源：http://qzq.havefunace.top

PHP:  array_count_values($arr);
来源：http://qmy.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://icq.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rbw.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ioo.snrcjt.cn

Go:   // 手写 map[T]int
来源：http://vcd.xinyue.icu

Ruby: arr.tally
来源：http://qqa.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vqn.yj202588.top

[D21] 判断是否包含某元素
来源：http://zvh.yongpay.top

Py:   x in arr
来源：http://ekj.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://owy.pycfn.com

JS:   arr.includes(x)
来源：http://igw.yj20258.top

TS:   arr.includes(x)
来源：http://odh.jianghu66.top

Java: list.contains(x)
来源：http://lui.aibaodan.cn

Go:   slices.Contains(arr, x)
来源：http://din.zhixingplan.top

Ruby: arr.include?(x)
来源：http://vzi.nwbrower.top

C#:   list.Contains(x)
来源：http://xgs.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://qec.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tex.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tql.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jrr.tarul.cn

TS:   [...arr];
来源：http://qik.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://sjm.mhx1999.top

Go:   copied := append([]int(nil), arr...)
来源：http://kwr.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://kua.cdnleiting.top

C#:   new List<int>(list);
来源：http://myf.daxiang520.top

[D23] reduce 累积计算
来源：http://nov.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lak.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://syd.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qfu.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kso.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mzn.gotoacloud.top

Go:   // 手写循环
来源：http://fbf.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ckw.pengpengdd.cyou

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gzy.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://lcc.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qii.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pii.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rla.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zqh.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ruv.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yzy.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xdg.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://htr.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://vnt.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qts.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vti.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fdm.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hsa.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fgs.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bik.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://scg.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ssm.ivvv.top

[D26] 数组转字符串
来源：http://xrl.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://kzo.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://bxr.ehwqpu.com

JS:   arr.join(", ")
来源：http://llp.hesvh.cn

TS:   arr.join(", ")
来源：http://xjt.ctjpmb.com

Java: String.join(", ", list)
来源：http://uzv.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://jyy.shuidangran.top

Ruby: arr.join(", ")
来源：http://nkm.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://tre.snrcjt.cn

================================================================================
来源：http://ixv.ydjk.org.cn

E. 字符串处理
来源：http://fbe.mhx1999.top

================================================================================
来源：http://lgm.zycfv.cn

[E01] 拼接字符串
来源：http://obv.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tzm.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baw.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qkz.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://njq.jqgfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bbr.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cdy.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aju.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jfg.fanxiaobao.xyz

[E02] 重复字符串
来源：http://sga.gaohongyu789.top

Py:   "ab" * 3
来源：http://dee.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://gyr.tarul.cn

JS:   "ab".repeat(3)
来源：http://ldq.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://zqr.shuidangran.top

Java: "ab".repeat(3)
来源：http://tow.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://ztv.yuanzhike.top

Ruby: "ab" * 3
来源：http://gdl.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sni.svipenyu.cn

[E03] 截取子串
来源：http://nvt.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://skv.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://chi.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ouj.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://iai.yj202588.top

Java: s.substring(1, 4)
来源：http://zxd.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hkk.zycfv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://byy.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://jnt.sufxvd.cn

[E04] 查找子串位置
来源：http://sep.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://cjz.xuanzx.com

PHP:  strpos($s, "x");
来源：http://hqd.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lto.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://oxt.iojbl.cn

Java: s.indexOf("x")
来源：http://mnj.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://ank.yangfankeji.com

Ruby: s.index("x")
来源：http://cal.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://pyq.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gfb.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rbr.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nzk.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ppm.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hmc.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ffi.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hof.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pae.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nph.smart0.xyz

[E06] 替换子串
来源：http://ste.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tbx.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://dib.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wir.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://hwf.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rwq.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nyv.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://txt.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://rgd.jyoumei.cn

[E07] 按分隔符拆分
来源：http://vdj.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jra.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uqm.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qsw.yj20258888.top

TS:   s.split(",")
来源：http://qba.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://tfu.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yvd.yonumen.top

Ruby: s.split(",");  s.split
来源：http://nte.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mfb.hnqzz.top

[E08] 数组按分隔符合并
来源：http://eyw.jinqigfzy.top

Py:   ",".join(items)
来源：http://gpt.yj20258.top

PHP:  implode(",", $items);
来源：http://zft.fktsv.cn

JS:   items.join(",")
来源：http://fvx.jianghu66.top

TS:   items.join(",")
来源：http://tqy.hnxiangtu.top

Java: String.join(",", items)
来源：http://ndv.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://pen.0kj1m.cn

Ruby: items.join(",")
来源：http://eou.tanke756.top

C#:   string.Join(",", items)
来源：http://dxe.yfazqb.com

[E09] 去除所有空白字符
来源：http://czi.jinqigufen.top


<!-- 参考信息 -->