代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://gtu.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://urs.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://svh.ybcxt.top

[D02] 追加元素到末尾
来源：http://kou.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fvb.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kcz.hywenlv.cn

JS:   arr.push(4);
来源：http://jlz.jqgfzy.top

TS:   arr.push(4);
来源：http://qaj.sxryk.cn

Java: list.add(4);
来源：http://hqf.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://okv.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://vax.nwbrower.top

C#:   list.Add(4);
来源：http://plv.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://kxh.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://ffg.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://avx.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zdu.yonumen.top

TS:   arr.splice(0, 0, 0);
来源：http://aut.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://bad.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aaw.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://frn.kuanghao11.cn

C#:   list.Insert(0, 0);
来源：http://jrl.tarul.cn

[D04] 删除元素
来源：http://awi.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kxu.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cro.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://azl.bbcook.cn

TS:   arr.splice(0, 1);
来源：http://ptj.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xoi.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bfv.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fmx.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xcp.tian-w.cn

[D05] 访问与修改元素
来源：http://mst.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ltd.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ver.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wwz.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://cov.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://ztv.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://zej.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cen.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://axd.tian-w.cn

[D06] 数组长度
来源：http://ygd.yj20258888.top

Py:   len(arr)
来源：http://kpf.ivvv.top

PHP:  count($arr);
来源：http://els.hammf.cn

JS:   arr.length
来源：http://wdl.vehdjk.com

TS:   arr.length
来源：http://pqg.guannengcc.top

Java: list.size();
来源：http://wzw.svipenyu.cn

Go:   len(arr)
来源：http://eug.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://gqo.cheryme.top

C#:   list.Count;
来源：http://pxt.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://ivk.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ato.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://zxh.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://jhd.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://dmm.hesvh.cn

Java: list.subList(1, 4);
来源：http://zxs.cheryme.top

Go:   arr[1:4]
来源：http://idj.hywenlv.cn

Ruby: arr[1, 3]
来源：http://sbz.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://lbd.cqqwz.cn

[D08] 合并两个数组
来源：http://qzr.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://qjl.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://bqx.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dfo.redwolf501.top

TS:   [...a, ...b];
来源：http://amq.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kvu.c1oappe.top

Go:   append(a, b...)
来源：http://etw.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://bjp.vqdsnc.cn

C#:   a.Concat(b).ToList()
来源：http://rmv.tianlin.xyz

[D09] 排序（升序）
来源：http://jwj.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://xrp.wangdashe.top

PHP:  sort($arr);
来源：http://bkq.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qgz.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://kcr.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://jsl.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aiv.svipenyu.cn

Ruby: arr.sort
来源：http://qgn.ydjk.org.cn

C#:   list.Sort();
来源：http://noq.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mgo.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lgd.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://giz.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lrj.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dxn.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iyo.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ajl.xuanzx.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yfd.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yyp.quarkkingdee.top

[D11] 反转数组
来源：http://kha.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mry.yfazqb.com

PHP:  array_reverse($arr);
来源：http://rxq.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mrk.xinyue.icu

TS:   [...arr].reverse();
来源：http://txk.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://oxi.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://lks.shuidangran.top

Ruby: arr.reverse
来源：http://moq.redwolf501.top

C#:   list.Reverse();
来源：http://mmu.shuidangran.top

[D12] 查找元素下标
来源：http://vbq.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://lwy.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ulu.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jsc.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zwy.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dsz.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://bde.9152youxi.cn

Ruby: arr.index(x)
来源：http://orb.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://aik.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://frq.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cyb.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oys.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://awd.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://pxx.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sbz.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hkh.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://zzf.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fka.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://oin.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://azw.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kbw.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://ovs.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://gom.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vvx.c1oappe.top

Go:   // 手写循环
来源：http://keh.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kpa.yj202588.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bpe.zhoulong.xyz

[D15] 去重
来源：http://rrj.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qap.yongpay.top

PHP:  array_unique($arr);
来源：http://bof.xziqi.cn

JS:   [...new Set(arr)]
来源：http://rjg.xylfe.cn

TS:   [...new Set(arr)]
来源：http://pfo.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pfe.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://vpv.shzxlz.cn

Ruby: arr.uniq
来源：http://epw.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://avq.yanxiufei.cn

[D16] 求和与平均值
来源：http://azx.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hme.0kj1m.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rti.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ogc.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://akz.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eqk.yfazqb.com

Go:   // 手写循环累加
来源：http://ncu.tianlin.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sid.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://gbr.gzhubu.top

[D17] 最大值与最小值
来源：http://wlb.yongpay.top

Py:   max(arr);  min(arr)
来源：http://dta.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://hoa.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wiz.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://cnw.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gma.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qww.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://mdi.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://axm.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://mty.zdqjudy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oxz.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://wby.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nfh.52xcode.cn

TS:   nested.flat();
来源：http://jfs.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://phv.9152youxi.cn

Go:   // 手写双层循环
来源：http://asw.c1oappe.top

Ruby: nested.flatten
来源：http://fdw.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pgp.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://fah.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kxe.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hbw.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://klt.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xal.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cdf.cashguo.top

Go:   // 手写 map[string][]T
来源：http://qeg.quarkkingdee.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://onf.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ana.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://wpb.fehbvm.com

Py:   Counter(arr)
来源：http://bpd.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://bdf.guowangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hcb.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yka.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yas.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://oek.shangyingyoupin.top

Ruby: arr.tally
来源：http://gsg.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cgn.pycfn.com

[D21] 判断是否包含某元素
来源：http://dlt.guannengcc.top

Py:   x in arr
来源：http://ssf.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://enp.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://oba.fengsongda.top

TS:   arr.includes(x)
来源：http://ffo.guowangkeji.top

Java: list.contains(x)
来源：http://rom.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://mwo.gotoacloud.top

Ruby: arr.include?(x)
来源：http://acv.yuanzhike.top

C#:   list.Contains(x)
来源：http://kmk.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://fse.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://afj.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://spm.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kqe.ctjpmb.com

TS:   [...arr];
来源：http://iok.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://fez.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://oir.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://eth.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://xvu.sxryk.cn

[D23] reduce 累积计算
来源：http://awt.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yfh.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qhj.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://irx.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gyv.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://fol.shangyingyoupin.top

Go:   // 手写循环
来源：http://sit.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jjt.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wgn.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://ewh.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rcm.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ihv.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vlm.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kbz.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ihy.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://slu.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://diu.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kgr.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://vcn.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yol.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xbn.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bjv.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mkd.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cvt.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fvb.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gac.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bym.0kj1m.cn

[D26] 数组转字符串
来源：http://dbs.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://zrg.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://jom.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://lof.shangyingyoupin.top

TS:   arr.join(", ")
来源：http://lrg.hammf.cn

Java: String.join(", ", list)
来源：http://sss.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://fhl.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://jhr.hesvh.cn

C#:   string.Join(", ", list)
来源：http://dbp.yueranfly.top

================================================================================
来源：http://gtm.gaohongyu789.top

E. 字符串处理
来源：http://rdf.xinyue.icu

================================================================================
来源：http://jlu.sysykeji.top

[E01] 拼接字符串
来源：http://ufk.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rhm.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fid.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tgi.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dgh.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bhm.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://inu.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yvm.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://opk.hnxiangtu.top

[E02] 重复字符串
来源：http://rjx.yongpay.top

Py:   "ab" * 3
来源：http://xud.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://yto.sweek.top

JS:   "ab".repeat(3)
来源：http://dgl.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://zdw.hysaishi.cn

Java: "ab".repeat(3)
来源：http://wbc.havefunace.top

Go:   strings.Repeat("ab", 3)
来源：http://rvj.hcnkem.com

Ruby: "ab" * 3
来源：http://mky.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fgg.zhongyouzk.top

[E03] 截取子串
来源：http://sma.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vup.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ucv.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lvg.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://ufj.zdbjq.cn

Java: s.substring(1, 4)
来源：http://dmw.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uum.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://acq.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://cqy.xuanzx.com

[E04] 查找子串位置
来源：http://iee.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://qvd.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://udl.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ibz.andypj.xyz

TS:   s.indexOf("x")
来源：http://zpd.tianlin.xyz

Java: s.indexOf("x")
来源：http://bjm.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://ibe.ydzc1.top

Ruby: s.index("x")
来源：http://hyi.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://atc.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://imy.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pxt.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://stx.hongshengwenyu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bgm.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://afn.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uxc.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wjo.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ibc.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kbw.shuidangran.top

[E06] 替换子串
来源：http://vix.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xbx.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://xoi.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qvw.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://uyl.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://itg.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://umd.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://reo.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://amr.havefunace.top

[E07] 按分隔符拆分
来源：http://cuh.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qws.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rvf.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://oek.ehwqpu.com

TS:   s.split(",")
来源：http://jig.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://urk.sjlbkw.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gdi.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://hbx.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tie.bjfxy.top

[E08] 数组按分隔符合并
来源：http://fzp.aibaodan.cn

Py:   ",".join(items)
来源：http://dsb.hcnkem.com

PHP:  implode(",", $items);
来源：http://yzi.snrcjt.cn

JS:   items.join(",")
来源：http://xqo.aizwys.cn

TS:   items.join(",")
来源：http://tpy.hcnkem.com

Java: String.join(",", items)
来源：http://ass.fzhhl.top


<!-- 参考信息 -->