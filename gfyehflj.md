代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://oax.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://roy.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mod.cdnleiting.top

================================================================================
来源：http://mua.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://ffi.ehwqpu.com

================================================================================
来源：http://glt.tarul.cn

[D01] 创建数组 / 列表
来源：http://xdz.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jpl.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://brc.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iom.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ibq.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yal.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://ooi.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://qsd.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mgh.tarul.cn

[D02] 追加元素到末尾
来源：http://mtf.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pxn.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zpd.gaohongyu789.top

JS:   arr.push(4);
来源：http://lsu.svipenyu.cn

TS:   arr.push(4);
来源：http://jcx.cdnleiting.top

Java: list.add(4);
来源：http://iek.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://zdk.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://fzw.hnqzz.top

C#:   list.Add(4);
来源：http://hjb.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://ygk.yj20258.top

Py:   arr.insert(0, 0)
来源：http://thr.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oiq.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://apz.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://qqc.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://izp.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://ycu.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sjn.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://dgq.cdnleiting.top

[D04] 删除元素
来源：http://mud.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jml.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://npo.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fvl.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://qqo.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tsm.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vpp.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lab.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uuh.xziqi.cn

[D05] 访问与修改元素
来源：http://jcf.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jlu.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fjf.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lsi.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://qim.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://ayr.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://gnr.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kgq.epnwcf.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zre.aizwys.cn

[D06] 数组长度
来源：http://vbe.tanke756.top

Py:   len(arr)
来源：http://vkt.hnqzz.top

PHP:  count($arr);
来源：http://wvo.guowangkeji.top

JS:   arr.length
来源：http://pnu.ywan-chungtsiang.top

TS:   arr.length
来源：http://etb.daxiang520.top

Java: list.size();
来源：http://xak.0kj1m.cn

Go:   len(arr)
来源：http://mhv.guannengcc.top

Ruby: arr.length; arr.size
来源：http://mdd.sjlbkw.cn

C#:   list.Count;
来源：http://fmz.gzhubu.top

[D07] 切片 / 取子数组
来源：http://hxw.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ajt.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://yjj.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://zfq.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://ivo.vehdjk.com

Java: list.subList(1, 4);
来源：http://rqp.xuetiantiany.cn

Go:   arr[1:4]
来源：http://scl.yuanzhike.top

Ruby: arr[1, 3]
来源：http://yat.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://prg.hammf.cn

[D08] 合并两个数组
来源：http://rnj.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://bmx.yfazqb.com

PHP:  array_merge($a, $b);
来源：http://ytc.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bbl.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://lqw.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://srk.cucudq.cn

Go:   append(a, b...)
来源：http://yiw.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://fdd.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://cvc.yongpay.top

[D09] 排序（升序）
来源：http://amk.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zts.shzxlz.cn

PHP:  sort($arr);
来源：http://xyn.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ide.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ijs.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gdl.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lbo.yj20258888.top

Ruby: arr.sort
来源：http://eny.sysykeji.top

C#:   list.Sort();
来源：http://mpg.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cfv.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ezu.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vuq.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jgg.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qff.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tst.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pat.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vgr.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yjt.sxryk.cn

[D11] 反转数组
来源：http://ibz.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://ava.sweek.top

PHP:  array_reverse($arr);
来源：http://liz.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://arc.sxryk.cn

TS:   [...arr].reverse();
来源：http://cfl.nanxinkj.top

Java: Collections.reverse(list);
来源：http://rsu.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://xsi.52xcode.cn

Ruby: arr.reverse
来源：http://xww.yuxming.cn

C#:   list.Reverse();
来源：http://uom.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://drb.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://eia.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://alo.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bnz.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chk.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://phq.cashguo.top

Go:   slices.Index(arr, x)
来源：http://pgd.shuidangran.top

Ruby: arr.index(x)
来源：http://jrt.redwolf501.top

C#:   list.IndexOf(x);
来源：http://qay.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://gfe.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bpr.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gix.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://puq.yuxming.cn

TS:   arr.filter(x => x > 3)
来源：http://rxr.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dng.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dlk.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://lma.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xht.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://ewh.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hxx.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xtb.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://yhx.9152youxi.cn

TS:   arr.map(x => x * 2)
来源：http://qyi.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://wwt.ybcxt.top

Go:   // 手写循环
来源：http://bzq.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://rjt.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ype.birdmap.top

[D15] 去重
来源：http://sbu.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uin.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://fpe.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://xak.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://arr.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://egj.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zoi.svipenyu.cn

Ruby: arr.uniq
来源：http://onw.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://qsa.fehbvm.com

[D16] 求和与平均值
来源：http://dtr.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://asf.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cmn.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lea.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rot.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iha.hcnkem.com

Go:   // 手写循环累加
来源：http://eub.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ycb.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://omj.0kj1m.cn

[D17] 最大值与最小值
来源：http://yjm.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://pgt.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://bjl.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cbh.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://ewa.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jgk.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pxs.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://ydr.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://nnx.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://rwd.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vou.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://exe.hnqzz.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nkq.ivvv.top

TS:   nested.flat();
来源：http://qab.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eiz.hammf.cn

Go:   // 手写双层循环
来源：http://jan.hammf.cn

Ruby: nested.flatten
来源：http://cfw.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oql.yangfankeji.com

[D19] 按字段分组
来源：http://xjw.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fte.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xis.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://usq.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://doj.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tjt.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://dok.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cir.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://khl.ivvv.top

[D20] 统计每个元素出现次数
来源：http://sdf.zhoulong.xyz

Py:   Counter(arr)
来源：http://zsc.yueranfly.top

PHP:  array_count_values($arr);
来源：http://ltl.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rkk.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jwh.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zsu.yongpay.top

Go:   // 手写 map[T]int
来源：http://psc.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://thp.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yjd.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://bcm.havefunace.top

Py:   x in arr
来源：http://cxy.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://kei.jinqigfzy.top

JS:   arr.includes(x)
来源：http://jol.vqdsnc.cn

TS:   arr.includes(x)
来源：http://vdw.guowangkeji.top

Java: list.contains(x)
来源：http://qqi.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://cyb.ppjwa.cn

Ruby: arr.include?(x)
来源：http://zhr.jianghu66.top

C#:   list.Contains(x)
来源：http://ytr.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://zpf.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://unl.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bwl.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://asj.xziqi.cn

TS:   [...arr];
来源：http://cem.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://liy.daxiang520.top

Go:   copied := append([]int(nil), arr...)
来源：http://eul.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://zph.quarkkingdee.top

C#:   new List<int>(list);
来源：http://toz.epnwcf.com

[D23] reduce 累积计算
来源：http://ovx.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cld.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bnc.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cuh.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mcr.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vmh.fehbvm.com

Go:   // 手写循环
来源：http://foo.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://npz.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nft.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://rjn.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bfw.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cop.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://azh.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cuy.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hft.shanyushiyangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qpr.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lnn.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bpp.havefunace.top

[D25] Set 集合去重与交并差
来源：http://rnl.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://juo.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gzq.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ona.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tpg.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ssh.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://krj.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iqc.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://awy.zhijiandao.cn

[D26] 数组转字符串
来源：http://nte.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://sny.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://bty.hnqzz.top

JS:   arr.join(", ")
来源：http://urb.zhongyouzk.top

TS:   arr.join(", ")
来源：http://oci.jyoumei.cn

Java: String.join(", ", list)
来源：http://yeu.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://jcl.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://qqe.aizwys.cn

C#:   string.Join(", ", list)
来源：http://lcr.yonumen.top

================================================================================
来源：http://ryw.yuanzhike.top

E. 字符串处理
来源：http://kds.ydzc1.top

================================================================================
来源：http://yfw.zdqjudy.top

[E01] 拼接字符串
来源：http://ecj.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zlj.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lbe.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uor.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fuy.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pgl.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ihm.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vqo.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mzi.jinqigfzy.top

[E02] 重复字符串
来源：http://ecl.yj20258.top

Py:   "ab" * 3
来源：http://wio.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://ite.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://mnb.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://fdb.snrcjt.cn

Java: "ab".repeat(3)
来源：http://vts.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://nes.dianchejie.cn

Ruby: "ab" * 3
来源：http://fzj.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hyk.fengsongda.top

[E03] 截取子串
来源：http://mrs.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hso.yvedp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wop.nanxuanxn.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hfp.yuxming.cn

TS:   s.slice(1, 4)
来源：http://mon.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://imb.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lfa.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yxp.yonumen.top

C#:   s.Substring(1, 3)
来源：http://mhl.gotoacloud.top

[E04] 查找子串位置
来源：http://sdq.jiagoushi.top

Py:   s.find("x");  s.index("x")
来源：http://nfg.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://axe.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nbw.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://kfx.jqgufenzy.top

Java: s.indexOf("x")
来源：http://eln.sweek.top

Go:   strings.Index(s, "x")
来源：http://zwl.yangfankeji.com

Ruby: s.index("x")
来源：http://kvv.tanke756.top

C#:   s.IndexOf("x")
来源：http://nqe.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dzm.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dup.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mam.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ptj.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://niv.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dte.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://puy.fehbvm.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ded.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://orv.yvedp.cn

[E06] 替换子串
来源：http://iwo.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kdg.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://qya.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://izv.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://npp.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vij.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cqe.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nwc.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://xea.ybcxt.top

[E07] 按分隔符拆分
来源：http://kuq.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xni.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rtu.nanxinkj.top


<!-- 参考信息 -->