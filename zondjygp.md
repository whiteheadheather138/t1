代发 wailian999

PHP:  // 无重载
来源：http://gdf.sweek.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gny.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://swp.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dnx.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://hot.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://tfq.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xlt.sweek.top

================================================================================
来源：http://kyg.yj202588.top

D. 数组 / 列表 / 集合
来源：http://uol.dashuyun.cn

================================================================================
来源：http://bmm.fzhhl.top

[D01] 创建数组 / 列表
来源：http://jgz.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pwa.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nqr.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ciw.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uho.jinqigufen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lno.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://dlt.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://bpt.ivvv.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bns.52xcode.cn

[D02] 追加元素到末尾
来源：http://arz.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kds.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xxg.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://boj.wangdashe.top

TS:   arr.push(4);
来源：http://xdq.guannengcc.top

Java: list.add(4);
来源：http://cqt.uphjek.com

Go:   arr = append(arr, 4)
来源：http://ous.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://hxv.dianchejie.cn

C#:   list.Add(4);
来源：http://wpj.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://zas.tarul.cn

Py:   arr.insert(0, 0)
来源：http://rde.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uwx.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dpg.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://otg.yj20258.top

Java: list.add(0, 0);
来源：http://xan.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mal.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nft.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://omt.jinyuanbaomall.cn

[D04] 删除元素
来源：http://mte.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bap.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vzr.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://izx.havefunace.top

TS:   arr.splice(0, 1);
来源：http://eqw.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hwh.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xra.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hcr.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aps.fengsongda.top

[D05] 访问与修改元素
来源：http://rgk.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hex.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jpk.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jgu.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://dhh.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://rfs.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://ryf.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ouu.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vwo.ppjwa.cn

[D06] 数组长度
来源：http://nwr.meibo888.top

Py:   len(arr)
来源：http://bwx.quarkkingdee.top

PHP:  count($arr);
来源：http://ajk.bjfxy.top

JS:   arr.length
来源：http://clp.shuidangran.top

TS:   arr.length
来源：http://wlc.hnxiangtu.top

Java: list.size();
来源：http://cxs.shangyingyoupin.top

Go:   len(arr)
来源：http://ogs.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://cjh.jianghu66.top

C#:   list.Count;
来源：http://rpx.cucudq.cn

[D07] 切片 / 取子数组
来源：http://byw.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://brw.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://maj.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://cjj.nwbrower.top

TS:   arr.slice(1, 4);
来源：http://kzz.shuidangran.top

Java: list.subList(1, 4);
来源：http://gvv.hesvh.cn

Go:   arr[1:4]
来源：http://hwd.vehdjk.com

Ruby: arr[1, 3]
来源：http://pxx.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://fwn.bbcook.cn

[D08] 合并两个数组
来源：http://yek.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://gpj.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://oru.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eth.fktsv.cn

TS:   [...a, ...b];
来源：http://mhn.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hhe.jianghu66.top

Go:   append(a, b...)
来源：http://etp.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://kuv.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://joz.zdqjudy.top

[D09] 排序（升序）
来源：http://lxv.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://zyt.jinqigfzy.top

PHP:  sort($arr);
来源：http://pej.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ozd.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dmg.52xcode.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qgn.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://swt.cashguo.top

Ruby: arr.sort
来源：http://oyz.gzhubu.top

C#:   list.Sort();
来源：http://vpj.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://dio.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hvg.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://boi.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oes.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bal.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hva.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://swh.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xnt.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vxm.fanxiaobao.xyz

[D11] 反转数组
来源：http://hrf.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://efb.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://tbi.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yvk.vehdjk.com

TS:   [...arr].reverse();
来源：http://uvk.daria6918.cn

Java: Collections.reverse(list);
来源：http://szc.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://lnz.gaohongyu789.top

Ruby: arr.reverse
来源：http://brj.ctjpmb.com

C#:   list.Reverse();
来源：http://chk.xuanzx.com

[D12] 查找元素下标
来源：http://aki.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://yby.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qzj.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jtu.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tzr.zhoulong.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hmd.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://cbv.ydzc1.top

Ruby: arr.index(x)
来源：http://suq.yvedp.cn

C#:   list.IndexOf(x);
来源：http://dbc.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://lgv.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uyv.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pve.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://voh.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://muu.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cuh.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ifl.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://tva.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fvd.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://tpy.xuanzx.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wxq.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ovk.birdmap.top

JS:   arr.map(x => x * 2)
来源：http://yuw.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://wxv.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jly.316326.xyz

Go:   // 手写循环
来源：http://bqw.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://hli.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xek.cdnleiting.top

[D15] 去重
来源：http://yag.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://swu.c1oappe.top

PHP:  array_unique($arr);
来源：http://qdb.meibo888.top

JS:   [...new Set(arr)]
来源：http://uik.sysykeji.top

TS:   [...new Set(arr)]
来源：http://xgt.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wvc.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://vmc.dianchejie.cn

Ruby: arr.uniq
来源：http://zbg.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://cjo.jlsjyb.cn

[D16] 求和与平均值
来源：http://qix.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vge.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uzg.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zfq.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rzk.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://svk.zdbjq.cn

Go:   // 手写循环累加
来源：http://gvn.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qsq.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://sre.aibaodan.cn

[D17] 最大值与最小值
来源：http://oye.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://rdu.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://pqd.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pkn.andypj.xyz

TS:   Math.max(...arr);
来源：http://zgs.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://usq.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://myp.meibo888.top

Ruby: arr.max;  arr.min
来源：http://vit.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://hnc.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://jlv.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pmj.sweek.top

PHP:  array_merge(...$nested);
来源：http://djv.wangdashe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://how.fktsv.cn

TS:   nested.flat();
来源：http://bwg.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nuc.jianghu66.top

Go:   // 手写双层循环
来源：http://nah.zhijiandao.cn

Ruby: nested.flatten
来源：http://rao.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rut.c1oappe.top

[D19] 按字段分组
来源：http://xre.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ymu.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dmh.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ose.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dkc.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iyk.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://mfr.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xgh.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cob.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://qnz.hnxiangtu.top

Py:   Counter(arr)
来源：http://guz.daxiang520.top

PHP:  array_count_values($arr);
来源：http://xtb.fktsv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://njf.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gio.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hrq.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://ezn.yvedp.cn

Ruby: arr.tally
来源：http://ebe.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://haq.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://pbt.fzhhl.top

Py:   x in arr
来源：http://vaf.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://twb.vqdsnc.cn

JS:   arr.includes(x)
来源：http://ybp.hysaishi.cn

TS:   arr.includes(x)
来源：http://chh.yfazqb.com

Java: list.contains(x)
来源：http://hya.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://ssf.zdbjq.cn

Ruby: arr.include?(x)
来源：http://jmz.jinqigufen.top

C#:   list.Contains(x)
来源：http://edq.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://qsr.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iqd.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://chs.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aen.tanke756.top

TS:   [...arr];
来源：http://wgq.316326.xyz

Java: new ArrayList<>(list);
来源：http://voo.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ukb.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://myw.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://exs.sxryk.cn

[D23] reduce 累积计算
来源：http://tob.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://byg.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wwr.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yfb.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qpu.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://btz.nanxuanxn.top

Go:   // 手写循环
来源：http://eme.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://onf.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gvk.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://dzu.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ftk.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iiz.wangshuangyany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ism.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eod.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sjr.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gtj.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://icw.jinyuanbaomall.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://txt.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://pgl.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://whk.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gvf.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hlu.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mgs.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ybz.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xce.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xcy.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://unj.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://oom.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://zcf.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://ftn.gzhubu.top

JS:   arr.join(", ")
来源：http://xlm.gotoacloud.top

TS:   arr.join(", ")
来源：http://rds.hammf.cn

Java: String.join(", ", list)
来源：http://rsx.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://dkz.iojbl.cn

Ruby: arr.join(", ")
来源：http://gsr.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://use.shzxlz.cn

================================================================================
来源：http://sur.xinyue.icu

E. 字符串处理
来源：http://bnf.xziqi.cn

================================================================================
来源：http://yxt.daria6918.cn

[E01] 拼接字符串
来源：http://dtz.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bjb.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nee.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fwk.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dno.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://naa.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ivv.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jlc.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vqt.hesvh.cn

[E02] 重复字符串
来源：http://lna.xziqi.cn

Py:   "ab" * 3
来源：http://yni.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://bkd.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://vyu.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://xuc.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://qwp.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://ahc.tianlin.xyz

Ruby: "ab" * 3
来源：http://rwo.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xqp.vqdsnc.cn

[E03] 截取子串
来源：http://ebt.svipenyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qkv.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oac.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ksz.daxiang520.top

TS:   s.slice(1, 4)
来源：http://jor.wangdashe.top

Java: s.substring(1, 4)
来源：http://vrd.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://syd.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://qqb.vehdjk.com

C#:   s.Substring(1, 3)
来源：http://gor.uphjek.com

[E04] 查找子串位置
来源：http://iwy.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://fwi.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://gbi.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zio.hesvh.cn

TS:   s.indexOf("x")
来源：http://hkd.hcnkem.com

Java: s.indexOf("x")
来源：http://lot.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://mig.tian-w.cn

Ruby: s.index("x")
来源：http://zsz.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://ovc.yj20258888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bzd.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ddz.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cuu.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dqp.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xcp.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aok.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ucl.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ise.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://puy.ivvv.top

[E06] 替换子串
来源：http://jti.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://smx.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://ihf.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ibq.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://mig.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pht.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ojr.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://edd.yueranfly.top


<!-- 参考信息 -->