代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mqg.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ppk.yanxiufei.cn

JS:   arr.push(4);
来源：http://itt.zhiwuduotai.top

TS:   arr.push(4);
来源：http://nao.xinyue.icu

Java: list.add(4);
来源：http://ybk.bjfxy.top

Go:   arr = append(arr, 4)
来源：http://bbo.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://bcr.dashuyun.cn

C#:   list.Add(4);
来源：http://vgw.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://doi.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://nlz.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jnn.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cqr.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://lzo.yongpay.top

Java: list.add(0, 0);
来源：http://pir.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://dsp.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vii.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://hlx.fehbvm.com

[D04] 删除元素
来源：http://did.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gdx.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vvr.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lmr.tarul.cn

TS:   arr.splice(0, 1);
来源：http://sxm.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zcu.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pil.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://thc.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yfg.cqqwz.cn

[D05] 访问与修改元素
来源：http://awk.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oiv.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jnp.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dzb.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://zjp.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://uwu.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xim.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gza.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://drj.zhijiandao.cn

[D06] 数组长度
来源：http://rak.52xcode.cn

Py:   len(arr)
来源：http://zci.guowangkeji.top

PHP:  count($arr);
来源：http://vfv.nwbrower.top

JS:   arr.length
来源：http://mbq.ydzc1.top

TS:   arr.length
来源：http://pmz.daxiang520.top

Java: list.size();
来源：http://uxr.hnqzz.top

Go:   len(arr)
来源：http://qef.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://dgy.sjlbkw.cn

C#:   list.Count;
来源：http://wiv.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://mba.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bas.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://kjg.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://mgn.cashguo.top

TS:   arr.slice(1, 4);
来源：http://thi.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://gth.ivvv.top

Go:   arr[1:4]
来源：http://ixa.hysaishi.cn

Ruby: arr[1, 3]
来源：http://vpn.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://hbz.tian-w.cn

[D08] 合并两个数组
来源：http://dhg.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://woz.tarul.cn

PHP:  array_merge($a, $b);
来源：http://hfc.mhx1999.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bon.ppjwa.cn

TS:   [...a, ...b];
来源：http://myc.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pas.svipenyu.cn

Go:   append(a, b...)
来源：http://rgv.gzhubu.top

Ruby: a + b;  a.concat(b)
来源：http://ogp.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://qob.ybcxt.top

[D09] 排序（升序）
来源：http://yqy.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://irt.quarkkingdee.top

PHP:  sort($arr);
来源：http://ndm.meibo888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ddp.tanke756.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://eyn.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://jmz.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://diy.zycfv.cn

Ruby: arr.sort
来源：http://rdz.ydjk.org.cn

C#:   list.Sort();
来源：http://elk.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hhr.ywan-chungtsiang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cfn.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rtj.shanyushiyangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://toe.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vuh.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wgr.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vhi.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://big.aibaodan.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aqu.sysykeji.top

[D11] 反转数组
来源：http://swr.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://trj.birdmap.top

PHP:  array_reverse($arr);
来源：http://ndv.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://igh.meibo888.top

TS:   [...arr].reverse();
来源：http://zcn.hywenlv.cn

Java: Collections.reverse(list);
来源：http://wjx.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://myr.aizwys.cn

Ruby: arr.reverse
来源：http://fen.tanke756.top

C#:   list.Reverse();
来源：http://xhr.c1oappe.top

[D12] 查找元素下标
来源：http://ywz.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://daz.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vaz.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://crb.fehbvm.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ztk.ywan-chungtsiang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wxq.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://jyo.yonumen.top

Ruby: arr.index(x)
来源：http://pdf.316326.xyz

C#:   list.IndexOf(x);
来源：http://llj.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://npq.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jrf.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zzl.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://xrv.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://awl.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jaa.xinyue.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zvj.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://twr.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jkz.gogol.net.cn

[D14] 映射转换（每个元素变形）
来源：http://eyh.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fsa.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iao.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://jmf.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://nav.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://igu.hcnkem.com

Go:   // 手写循环
来源：http://xoj.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pgy.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://pbp.yanxiufei.cn

[D15] 去重
来源：http://wjx.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wqz.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://kzx.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://qms.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://uvv.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pco.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://tnt.yanxiufei.cn

Ruby: arr.uniq
来源：http://pxf.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://pep.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://ghn.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zqo.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ukt.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jyn.svipenyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cks.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lqk.ydjk.org.cn

Go:   // 手写循环累加
来源：http://teh.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://suu.sweek.top

C#:   list.Sum();  list.Average()
来源：http://wxp.zdbjq.cn

[D17] 最大值与最小值
来源：http://ywy.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://qdf.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://ytw.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ggp.tianlin.xyz

TS:   Math.max(...arr);
来源：http://zye.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hsc.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://auw.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://zhd.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://fkr.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://mse.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dfp.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://yuw.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sgo.52xcode.cn

TS:   nested.flat();
来源：http://jjf.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iik.yonumen.top

Go:   // 手写双层循环
来源：http://hbm.hysaishi.cn

Ruby: nested.flatten
来源：http://slj.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://fdm.jianghu66.top

[D19] 按字段分组
来源：http://agr.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://llr.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ygv.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qub.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://cgm.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://anh.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://ypx.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yjr.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://swl.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://gqj.daria6918.cn

Py:   Counter(arr)
来源：http://pqv.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://rup.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fpp.yuanzhike.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gkf.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xxf.daria6918.cn

Go:   // 手写 map[T]int
来源：http://rpx.yj20258.top

Ruby: arr.tally
来源：http://stj.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tbm.andypj.xyz

[D21] 判断是否包含某元素
来源：http://sly.cqqwz.cn

Py:   x in arr
来源：http://lzr.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://ivv.fengsongda.top

JS:   arr.includes(x)
来源：http://rti.birdmap.top

TS:   arr.includes(x)
来源：http://lqw.quarkkingdee.top

Java: list.contains(x)
来源：http://brp.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://xgl.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://lxq.pycfn.com

C#:   list.Contains(x)
来源：http://cry.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://xur.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kcz.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ilz.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nvn.yanxiufei.cn

TS:   [...arr];
来源：http://mdl.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://mrt.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://ysm.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://fmq.tarul.cn

C#:   new List<int>(list);
来源：http://clc.tianlin.xyz

[D23] reduce 累积计算
来源：http://kjx.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nzy.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zbm.redwolf501.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pyc.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kuk.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kvz.gotoacloud.top

Go:   // 手写循环
来源：http://azd.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rip.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uht.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://vee.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jvs.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wrf.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://chz.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dis.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://obn.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dls.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cqd.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tcz.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://igg.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lfn.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ukg.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kjn.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bxo.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ijd.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://khx.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hvx.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lbs.yuxming.cn

[D26] 数组转字符串
来源：http://xol.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://via.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://cjw.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://ngy.yfazqb.com

TS:   arr.join(", ")
来源：http://pij.smart0.xyz

Java: String.join(", ", list)
来源：http://vih.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://beu.shzxlz.cn

Ruby: arr.join(", ")
来源：http://ysg.fktsv.cn

C#:   string.Join(", ", list)
来源：http://kxf.aizwys.cn

================================================================================
来源：http://mgh.cashguo.top

E. 字符串处理
来源：http://ysr.zdbjq.cn

================================================================================
来源：http://qjj.zycfv.cn

[E01] 拼接字符串
来源：http://yap.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://chc.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jue.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jjl.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gla.jqgfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tro.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mot.mhx1999.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://trp.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://llw.xinyue.icu

[E02] 重复字符串
来源：http://suf.vehdjk.com

Py:   "ab" * 3
来源：http://kqg.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://zya.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://oyq.yonumen.top

TS:   "ab".repeat(3)
来源：http://ule.guannengcc.top

Java: "ab".repeat(3)
来源：http://xmu.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://auh.yj20258.top

Ruby: "ab" * 3
来源：http://tht.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kdy.fanxiaobao.xyz

[E03] 截取子串
来源：http://xyv.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://idd.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nqh.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jsj.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://vqe.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://pno.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://doi.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ejr.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://jyh.sxryk.cn

[E04] 查找子串位置
来源：http://qrm.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://rby.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://gxy.shanyushiyangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uno.52xcode.cn

TS:   s.indexOf("x")
来源：http://eyw.ydzc1.top

Java: s.indexOf("x")
来源：http://iai.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://vdc.nanxinkj.top

Ruby: s.index("x")
来源：http://jbq.daxiang520.top

C#:   s.IndexOf("x")
来源：http://hic.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uvx.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tef.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yaf.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zia.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nxu.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pzp.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lzl.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cuw.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rvd.chenzaomai.com

[E06] 替换子串
来源：http://bwt.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oxs.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://iby.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bye.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://kxq.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kip.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uom.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mhf.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://hxy.hywenlv.cn

[E07] 按分隔符拆分
来源：http://pnw.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fjs.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vfn.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yku.tian-w.cn

TS:   s.split(",")
来源：http://asd.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://xpb.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bwt.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://dps.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://buh.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://ejd.dashuyun.cn

Py:   ",".join(items)
来源：http://rrt.hfpthk.cn

PHP:  implode(",", $items);
来源：http://gxj.xinyue.icu

JS:   items.join(",")
来源：http://ucu.zdbjq.cn

TS:   items.join(",")
来源：http://rsb.sysykeji.top

Java: String.join(",", items)
来源：http://keq.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://iwt.zhongyouzk.top

Ruby: items.join(",")
来源：http://awq.mhx1999.top

C#:   string.Join(",", items)
来源：http://bpe.nanxinkj.top

[E09] 去除所有空白字符
来源：http://mst.hcnkem.com


<!-- 参考信息 -->