代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://oia.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://fpu.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://rcu.yonumen.top

================================================================================
来源：http://rzj.birdmap.top

D. 数组 / 列表 / 集合
来源：http://qmk.shzxlz.cn

================================================================================
来源：http://thg.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://tdz.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://clm.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rcc.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lfl.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ehu.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vin.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://iqt.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://yiy.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rzp.jianghu66.top

[D02] 追加元素到末尾
来源：http://pna.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yoc.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mwz.jyoumei.cn

JS:   arr.push(4);
来源：http://pfo.xuetiantiany.cn

TS:   arr.push(4);
来源：http://ayh.xylfe.cn

Java: list.add(4);
来源：http://cpg.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://lrp.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://mds.hnqzz.top

C#:   list.Add(4);
来源：http://zpz.yj20258888.top

[D03] 在指定位置插入元素
来源：http://dhv.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://rlq.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mvh.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pje.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://qth.ctjpmb.com

Java: list.add(0, 0);
来源：http://jxv.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jui.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gsx.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://jtz.xuetiantiany.cn

[D04] 删除元素
来源：http://nta.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mcs.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eua.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jio.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://rzj.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ipg.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://znh.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://icr.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jel.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://wim.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://coa.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://szs.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tfm.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://tkz.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://sxc.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://laa.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pjz.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zic.andypj.xyz

[D06] 数组长度
来源：http://cip.zhengqikj.top

Py:   len(arr)
来源：http://wro.fzhhl.top

PHP:  count($arr);
来源：http://imt.zdbjq.cn

JS:   arr.length
来源：http://uux.zdqjudy.top

TS:   arr.length
来源：http://ygt.chenlongwang.top

Java: list.size();
来源：http://zlk.jqgufenzy.top

Go:   len(arr)
来源：http://jyr.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://gdi.quarkkingdee.top

C#:   list.Count;
来源：http://sys.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://jqv.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cii.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://hue.yonumen.top

JS:   arr.slice(1, 4);
来源：http://cyx.havefunace.top

TS:   arr.slice(1, 4);
来源：http://fgr.ivvv.top

Java: list.subList(1, 4);
来源：http://nsp.jyoumei.cn

Go:   arr[1:4]
来源：http://xzk.hongshengwenyu.top

Ruby: arr[1, 3]
来源：http://ftz.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://xde.yanxiufei.cn

[D08] 合并两个数组
来源：http://lll.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://edg.fanxiaobao.xyz

PHP:  array_merge($a, $b);
来源：http://orm.andypj.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://hor.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://tdz.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zpv.dashuyun.cn

Go:   append(a, b...)
来源：http://ejb.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://lfa.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://omu.ivvv.top

[D09] 排序（升序）
来源：http://lta.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://mks.ydzc1.top

PHP:  sort($arr);
来源：http://dsv.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://imq.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lti.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://yzl.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ytl.dianchejie.cn

Ruby: arr.sort
来源：http://ypg.hcnkem.com

C#:   list.Sort();
来源：http://pki.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jqt.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rog.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aoi.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://clk.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pnj.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zmx.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://umi.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fjb.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://spr.hnqzz.top

[D11] 反转数组
来源：http://ypb.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ubc.hammf.cn

PHP:  array_reverse($arr);
来源：http://edb.hywenlv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mxt.tian-w.cn

TS:   [...arr].reverse();
来源：http://zpd.nwbrower.top

Java: Collections.reverse(list);
来源：http://wok.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://kkk.vqdsnc.cn

Ruby: arr.reverse
来源：http://xdk.fengsongda.top

C#:   list.Reverse();
来源：http://bay.quarkkingdee.top

[D12] 查找元素下标
来源：http://aav.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://miu.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bcl.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qxz.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hyx.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ceu.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://whv.zhixingplan.top

Ruby: arr.index(x)
来源：http://nbf.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://tpn.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://dgb.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mer.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uwg.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://oyb.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://ppz.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cne.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hto.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ltt.nwbrower.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cgn.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://trd.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wtm.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sje.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://pxr.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://zrs.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zdo.guannengcc.top

Go:   // 手写循环
来源：http://mqs.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://fce.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://geb.jlsjyb.cn

[D15] 去重
来源：http://gyg.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hmo.havefunace.top

PHP:  array_unique($arr);
来源：http://zuj.52xcode.cn

JS:   [...new Set(arr)]
来源：http://nnb.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://pqe.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://efi.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://iyn.sjlbkw.cn

Ruby: arr.uniq
来源：http://iwo.aizwys.cn

C#:   list.Distinct().ToList()
来源：http://asu.cheryme.top

[D16] 求和与平均值
来源：http://aka.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oug.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bcu.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fqm.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://izf.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kct.svipenyu.cn

Go:   // 手写循环累加
来源：http://giv.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://txa.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://thv.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://csw.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://psm.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://tfr.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dyi.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://fgh.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cib.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tal.pycfn.com

Ruby: arr.max;  arr.min
来源：http://boh.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://eyv.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://fbj.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rmv.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://hya.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gpj.xuanzx.com

TS:   nested.flat();
来源：http://cvq.ydjk.org.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://avm.vehdjk.com

Go:   // 手写双层循环
来源：http://lpb.sweek.top

Ruby: nested.flatten
来源：http://enw.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://owl.shzxlz.cn

[D19] 按字段分组
来源：http://hut.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vba.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://svv.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qdo.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://kbi.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ybi.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://dtl.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jid.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tvr.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://baz.chenlongwang.top

Py:   Counter(arr)
来源：http://zjp.52xcode.cn

PHP:  array_count_values($arr);
来源：http://vvs.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ayt.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://axi.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://foy.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://jrt.jiagoushi.top

Ruby: arr.tally
来源：http://oxs.yuanzhike.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uah.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://wyb.yj20258888.top

Py:   x in arr
来源：http://lug.ydzc1.top

PHP:  in_array($x, $arr, true);
来源：http://eym.xuanzx.com

JS:   arr.includes(x)
来源：http://waj.316326.xyz

TS:   arr.includes(x)
来源：http://lth.haohaochexian.top

Java: list.contains(x)
来源：http://jhb.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://bbn.jqgfzy.top

Ruby: arr.include?(x)
来源：http://jfi.jinqigufen.top

C#:   list.Contains(x)
来源：http://ilb.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://eeg.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lfl.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://exu.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qei.dianchejie.cn

TS:   [...arr];
来源：http://ifd.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://dsz.pycfn.com

Go:   copied := append([]int(nil), arr...)
来源：http://hqn.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://dna.meibo888.top

C#:   new List<int>(list);
来源：http://vis.hcnkem.com

[D23] reduce 累积计算
来源：http://biq.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qag.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eyl.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pxn.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qxd.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://pze.yvedp.cn

Go:   // 手写循环
来源：http://ier.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dge.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zhc.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://owk.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ftd.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qwg.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sjz.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lmi.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pzb.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pxj.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tfm.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://slf.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://aqy.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nfj.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://num.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bhq.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hgw.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nqr.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bwt.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tdo.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zoc.cheryme.top

[D26] 数组转字符串
来源：http://bxp.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://zld.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://ivs.yj20258.top

JS:   arr.join(", ")
来源：http://qnn.yangfankeji.com

TS:   arr.join(", ")
来源：http://ikk.yonumen.top

Java: String.join(", ", list)
来源：http://jhx.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://qap.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://uso.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://wmg.shuidangran.top

================================================================================
来源：http://yvr.svipenyu.cn

E. 字符串处理
来源：http://hvq.tian-w.cn

================================================================================
来源：http://jvs.9152youxi.cn

[E01] 拼接字符串
来源：http://nsc.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rfn.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://skt.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lbv.tanke756.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zkn.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://exn.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uah.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uit.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yxu.ydjk.org.cn

[E02] 重复字符串
来源：http://tax.shzxlz.cn

Py:   "ab" * 3
来源：http://urx.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://zpa.hesvh.cn

JS:   "ab".repeat(3)
来源：http://skj.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://nnl.chenzaomai.com

Java: "ab".repeat(3)
来源：http://rrg.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://twc.daria6918.cn

Ruby: "ab" * 3
来源：http://rgm.wangshuangyany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jhh.uphjek.com

[E03] 截取子串
来源：http://uoi.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://trm.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jir.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://srx.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://bbb.xuanzx.com

Java: s.substring(1, 4)
来源：http://nem.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://asc.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lti.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://jzi.svipenyu.cn

[E04] 查找子串位置
来源：http://gqv.hnxiangtu.top

Py:   s.find("x");  s.index("x")
来源：http://hvq.yj20258.top

PHP:  strpos($s, "x");
来源：http://lug.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kzo.gzhubu.top

TS:   s.indexOf("x")
来源：http://qou.wangdashe.top

Java: s.indexOf("x")
来源：http://kxq.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://uqg.aibaodan.cn

Ruby: s.index("x")
来源：http://oba.hesvh.cn

C#:   s.IndexOf("x")
来源：http://yxd.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rup.nwbrower.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xcc.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hdo.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ikg.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://odm.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mro.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://flp.zhaomingkeji.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lyh.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kil.yuxming.cn

[E06] 替换子串
来源：http://kze.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bha.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://wvo.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://puk.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://jut.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iay.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pxv.cdnleiting.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ozq.birdmap.top

C#:   s.Replace("a", "b")
来源：http://vuj.zhijiandao.cn

[E07] 按分隔符拆分
来源：http://egq.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ecz.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qsu.zhoulong.xyz


<!-- 参考信息 -->