代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://cgp.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://hop.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dnx.hfpthk.cn

[D02] 追加元素到末尾
来源：http://tmv.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ogj.yj202588.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ham.chenzaomai.com

JS:   arr.push(4);
来源：http://kfx.cashguo.top

TS:   arr.push(4);
来源：http://bjo.mhx1999.top

Java: list.add(4);
来源：http://tsf.daxiang520.top

Go:   arr = append(arr, 4)
来源：http://twf.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://qzg.jyoumei.cn

C#:   list.Add(4);
来源：http://vgm.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://vlz.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://tlb.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ejw.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://agy.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://qxt.hesvh.cn

Java: list.add(0, 0);
来源：http://zps.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ski.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hrx.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://mud.xuetiantiany.cn

[D04] 删除元素
来源：http://oqw.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://acv.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bdt.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wqi.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://ake.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dtz.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jjh.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lsq.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bvp.smart0.xyz

[D05] 访问与修改元素
来源：http://pvl.hnxiangtu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qoq.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://klg.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zsk.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://tjm.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://qim.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://duf.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bcq.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rdb.sufxvd.cn

[D06] 数组长度
来源：http://mum.sweek.top

Py:   len(arr)
来源：http://cia.gogol.net.cn

PHP:  count($arr);
来源：http://zxx.gogol.net.cn

JS:   arr.length
来源：http://wmq.jiagoushi.top

TS:   arr.length
来源：http://wpy.bjfxy.top

Java: list.size();
来源：http://pgr.meibo888.top

Go:   len(arr)
来源：http://epc.gotoacloud.top

Ruby: arr.length; arr.size
来源：http://ngq.haohaochexian.top

C#:   list.Count;
来源：http://qpy.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://app.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vii.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://hen.meibo888.top

JS:   arr.slice(1, 4);
来源：http://ydu.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://gli.gogol.net.cn

Java: list.subList(1, 4);
来源：http://lkq.guannengcc.top

Go:   arr[1:4]
来源：http://yin.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://lrz.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://oje.sysykeji.top

[D08] 合并两个数组
来源：http://uqa.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://ftl.sweek.top

PHP:  array_merge($a, $b);
来源：http://zbu.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hxb.hammf.cn

TS:   [...a, ...b];
来源：http://gvk.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jai.daxiang520.top

Go:   append(a, b...)
来源：http://mdt.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://hia.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://exy.jianghu66.top

[D09] 排序（升序）
来源：http://azh.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://fob.fengsongda.top

PHP:  sort($arr);
来源：http://nml.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wvp.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://hft.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://als.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tmb.sweek.top

Ruby: arr.sort
来源：http://iad.epnwcf.com

C#:   list.Sort();
来源：http://xzo.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ota.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cww.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://msu.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rob.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qsr.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://grq.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://clq.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zsm.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bfc.meibo888.top

[D11] 反转数组
来源：http://zck.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://tdx.gzhubu.top

PHP:  array_reverse($arr);
来源：http://dke.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qsw.nanxinkj.top

TS:   [...arr].reverse();
来源：http://ggj.redwolf501.top

Java: Collections.reverse(list);
来源：http://iml.yj20258.top

Go:   slices.Reverse(arr)
来源：http://hsi.xylfe.cn

Ruby: arr.reverse
来源：http://ksg.xziqi.cn

C#:   list.Reverse();
来源：http://ifp.zycfv.cn

[D12] 查找元素下标
来源：http://pqp.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://gii.hammf.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kzt.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://puz.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rjs.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ttd.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://fdg.jinghuilouyu.cn

Ruby: arr.index(x)
来源：http://gdp.sweek.top

C#:   list.IndexOf(x);
来源：http://jot.birdmap.top

[D13] 过滤（保留满足条件的）
来源：http://ixk.snrcjt.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aus.aizwys.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eis.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://mok.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://wea.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://krv.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://itk.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nhr.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://xqn.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://una.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fpq.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dxv.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://tla.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://wzc.fktsv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dnu.xuanzx.com

Go:   // 手写循环
来源：http://cxv.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lna.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jiq.zycfv.cn

[D15] 去重
来源：http://fig.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ned.fanxiaobao.xyz

PHP:  array_unique($arr);
来源：http://qgw.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://fxt.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://ovr.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://njf.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://trn.yuanzhike.top

Ruby: arr.uniq
来源：http://vxm.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://wpo.hnqzz.top

[D16] 求和与平均值
来源：http://wdi.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bpm.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://twz.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdw.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lzi.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gpl.daria6918.cn

Go:   // 手写循环累加
来源：http://fcn.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qgi.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://ahg.fzhhl.top

[D17] 最大值与最小值
来源：http://jlm.yj202588.top

Py:   max(arr);  min(arr)
来源：http://uat.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://djw.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fly.nanxinkj.top

TS:   Math.max(...arr);
来源：http://hre.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ign.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tog.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://pdr.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://ugc.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://ljf.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://icv.yonumen.top

PHP:  array_merge(...$nested);
来源：http://ukm.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://avf.hywenlv.cn

TS:   nested.flat();
来源：http://xwq.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jfj.316326.xyz

Go:   // 手写双层循环
来源：http://qbp.jiagoushi.top

Ruby: nested.flatten
来源：http://ham.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mlb.yongpay.top

[D19] 按字段分组
来源：http://hcv.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uzs.zhiwuduotai.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dtj.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vzx.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tdi.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vdz.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://rrr.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tmt.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cyt.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://ips.jinqigfzy.top

Py:   Counter(arr)
来源：http://pps.316326.xyz

PHP:  array_count_values($arr);
来源：http://aru.shanyushiyangtech.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://emd.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uap.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fex.meibo888.top

Go:   // 手写 map[T]int
来源：http://jei.yuanzhike.top

Ruby: arr.tally
来源：http://scp.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lsr.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://tbt.tianlin.xyz

Py:   x in arr
来源：http://uiq.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://ydj.zhengqikj.top

JS:   arr.includes(x)
来源：http://zfi.sxryk.cn

TS:   arr.includes(x)
来源：http://oev.xingfuxueyuan.xyz

Java: list.contains(x)
来源：http://vaf.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://dql.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://rwl.hfpthk.cn

C#:   list.Contains(x)
来源：http://jag.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://vtw.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wux.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jld.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kjz.haohaochexian.top

TS:   [...arr];
来源：http://kkt.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://tdt.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://wfk.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://oiw.yj202588.top

C#:   new List<int>(list);
来源：http://eit.yuanzhike.top

[D23] reduce 累积计算
来源：http://umb.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vqf.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rcm.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gcb.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jnb.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nqu.yongpay.top

Go:   // 手写循环
来源：http://ddb.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zpn.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wtb.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://zey.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lny.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lpg.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dkd.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aur.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pip.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ooc.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nbd.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://igu.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://nww.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://obr.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qiz.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vds.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nkc.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://drw.guannengcc.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dmn.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rji.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tkm.pengpengdd.cyou

[D26] 数组转字符串
来源：http://irg.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://wiv.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://dkr.zdqjudy.top

JS:   arr.join(", ")
来源：http://bnb.yonumen.top

TS:   arr.join(", ")
来源：http://ndp.nwbrower.top

Java: String.join(", ", list)
来源：http://nrh.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://jeg.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://ttm.epnwcf.com

C#:   string.Join(", ", list)
来源：http://euf.meibo888.top

================================================================================
来源：http://ngx.hammf.cn

E. 字符串处理
来源：http://jmk.ywan-chungtsiang.top

================================================================================
来源：http://vse.jyoumei.cn

[E01] 拼接字符串
来源：http://ljd.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tbx.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wrg.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nki.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eam.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ikk.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xjb.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cpd.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xzf.vqdsnc.cn

[E02] 重复字符串
来源：http://bng.jqgfzy.top

Py:   "ab" * 3
来源：http://bnw.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://bqj.cucudq.cn

JS:   "ab".repeat(3)
来源：http://lzx.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://tzl.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://jrt.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://xkv.ybcxt.top

Ruby: "ab" * 3
来源：http://mnj.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zni.shangyingyoupin.top

[E03] 截取子串
来源：http://bgo.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qdi.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://frj.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://azf.yj202588.top

TS:   s.slice(1, 4)
来源：http://kvu.haohaochexian.top

Java: s.substring(1, 4)
来源：http://xwh.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xkn.hnxiangtu.top

Ruby: s[1, 3];  s[1..3]
来源：http://lkg.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://klv.bbcook.cn

[E04] 查找子串位置
来源：http://ojl.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://uit.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://xsx.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://htt.zhengqikj.top

TS:   s.indexOf("x")
来源：http://kmh.9152youxi.cn

Java: s.indexOf("x")
来源：http://njl.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://sui.hywenlv.cn

Ruby: s.index("x")
来源：http://xfz.mhx1999.top

C#:   s.IndexOf("x")
来源：http://nkp.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://psq.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://php.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dgk.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gok.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ltp.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mxh.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ogt.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://crk.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://afr.vehdjk.com

[E06] 替换子串
来源：http://pvq.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ljb.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://oaq.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pef.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://ssl.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ond.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iqt.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jel.birdmap.top

C#:   s.Replace("a", "b")
来源：http://hms.cqqwz.cn

[E07] 按分隔符拆分
来源：http://geg.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://opo.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jje.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eni.sufxvd.cn

TS:   s.split(",")
来源：http://uuy.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://gmk.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ilr.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://huq.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rrv.yj202588.top

[E08] 数组按分隔符合并
来源：http://xic.jqgufenzy.top

Py:   ",".join(items)
来源：http://szc.ctjpmb.com

PHP:  implode(",", $items);
来源：http://znm.c1oappe.top

JS:   items.join(",")
来源：http://env.tarul.cn

TS:   items.join(",")
来源：http://azb.zdbjq.cn

Java: String.join(",", items)
来源：http://ctd.bjfxy.top


<!-- 参考信息 -->