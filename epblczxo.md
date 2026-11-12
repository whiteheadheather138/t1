代发 wailian999

PHP:  // 无重载
来源：http://jlx.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://iom.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://kbo.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://neg.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://gkw.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://lue.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://npk.redwolf501.top

================================================================================
来源：http://lfw.cqqwz.cn

D. 数组 / 列表 / 集合
来源：http://gjk.hcnkem.com

================================================================================
来源：http://rhr.guowangkeji.top

[D01] 创建数组 / 列表
来源：http://uwq.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jcf.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aus.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uka.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xnd.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nfz.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://arf.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://ied.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ozo.yfazqb.com

[D02] 追加元素到末尾
来源：http://sex.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qkv.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://juw.jqgufenzy.top

JS:   arr.push(4);
来源：http://jwu.jiagoushi.top

TS:   arr.push(4);
来源：http://wci.ydjk.org.cn

Java: list.add(4);
来源：http://ylt.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://lcx.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://akz.chenzaomai.com

C#:   list.Add(4);
来源：http://fpp.nwbrower.top

[D03] 在指定位置插入元素
来源：http://dcv.birdmap.top

Py:   arr.insert(0, 0)
来源：http://jfm.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oqy.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qmj.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://gux.yfazqb.com

Java: list.add(0, 0);
来源：http://bct.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://vnu.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cet.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://erg.zhixingplan.top

[D04] 删除元素
来源：http://mzu.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bpo.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mjv.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pam.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://ojz.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://idu.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pee.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yuc.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xow.yj20258.top

[D05] 访问与修改元素
来源：http://ilr.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qdo.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zoz.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ccz.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://bqf.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://toq.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://gkn.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ivt.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zeh.sysykeji.top

[D06] 数组长度
来源：http://pxw.chenjidiqi.icu

Py:   len(arr)
来源：http://tgj.yangfankeji.com

PHP:  count($arr);
来源：http://nhf.chenjidiqi.icu

JS:   arr.length
来源：http://xvy.bjfxy.top

TS:   arr.length
来源：http://kuv.andypj.xyz

Java: list.size();
来源：http://ypw.xuetiantiany.cn

Go:   len(arr)
来源：http://wys.hcnkem.com

Ruby: arr.length; arr.size
来源：http://iqx.hammf.cn

C#:   list.Count;
来源：http://asx.xziqi.cn

[D07] 切片 / 取子数组
来源：http://vln.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hwq.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fsj.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://wyv.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://nux.hesvh.cn

Java: list.subList(1, 4);
来源：http://xbb.iojbl.cn

Go:   arr[1:4]
来源：http://wcx.andypj.xyz

Ruby: arr[1, 3]
来源：http://epv.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://cyx.fzhhl.top

[D08] 合并两个数组
来源：http://aga.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://nhl.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://nqy.ppjwa.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sjy.cheryme.top

TS:   [...a, ...b];
来源：http://miu.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nqc.jlsjyb.cn

Go:   append(a, b...)
来源：http://sto.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://zsg.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://gzv.fktsv.cn

[D09] 排序（升序）
来源：http://nyc.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://jun.nwbrower.top

PHP:  sort($arr);
来源：http://gea.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rgg.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://obq.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vkm.zycfv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ivp.xziqi.cn

Ruby: arr.sort
来源：http://cpi.epnwcf.com

C#:   list.Sort();
来源：http://beh.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://adm.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ams.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ted.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gom.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvv.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nyu.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vii.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://crv.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wpb.vehdjk.com

[D11] 反转数组
来源：http://ueg.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://wet.nwbrower.top

PHP:  array_reverse($arr);
来源：http://opf.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://skt.andypj.xyz

TS:   [...arr].reverse();
来源：http://yso.ehwqpu.com

Java: Collections.reverse(list);
来源：http://bbe.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://xul.ydzc1.top

Ruby: arr.reverse
来源：http://heh.wangdashe.top

C#:   list.Reverse();
来源：http://dzl.redwolf501.top

[D12] 查找元素下标
来源：http://cgt.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://idw.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rge.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://auv.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mzg.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zht.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://uyj.9152youxi.cn

Ruby: arr.index(x)
来源：http://mfr.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://ruk.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://ase.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lho.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vdk.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://rqa.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://ijx.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jff.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kfd.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://upe.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yij.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://oin.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sfb.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gcp.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://jqs.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://qol.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gkx.jqgfzy.top

Go:   // 手写循环
来源：http://bto.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nfk.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vwt.ctjpmb.com

[D15] 去重
来源：http://bag.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://axb.sysykeji.top

PHP:  array_unique($arr);
来源：http://mol.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://tcx.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://flw.hammf.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rjy.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://uqz.hnqzz.top

Ruby: arr.uniq
来源：http://quj.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://nka.nanxinkj.top

[D16] 求和与平均值
来源：http://tdn.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dby.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lth.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ejm.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nuc.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xcg.jyoumei.cn

Go:   // 手写循环累加
来源：http://wby.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://snd.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://sim.zhixingplan.top

[D17] 最大值与最小值
来源：http://qdw.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://tyn.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://bqu.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wyw.dianchejie.cn

TS:   Math.max(...arr);
来源：http://kja.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qvq.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pys.hammf.cn

Ruby: arr.max;  arr.min
来源：http://ilh.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://zzm.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://bik.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vzf.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://amo.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ncy.yj202588.top

TS:   nested.flat();
来源：http://amd.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xac.zdbjq.cn

Go:   // 手写双层循环
来源：http://jsy.meibo888.top

Ruby: nested.flatten
来源：http://unw.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lqc.sxryk.cn

[D19] 按字段分组
来源：http://ill.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://irs.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yqb.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rww.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uqe.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iax.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://jyv.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ykz.zhixingplan.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ybb.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://xhs.xylfe.cn

Py:   Counter(arr)
来源：http://vpv.ybcxt.top

PHP:  array_count_values($arr);
来源：http://gib.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ryu.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xvm.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://epe.cqqwz.cn

Go:   // 手写 map[T]int
来源：http://tkg.yuanzhike.top

Ruby: arr.tally
来源：http://tgk.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://czg.ybcxt.top

[D21] 判断是否包含某元素
来源：http://rsm.pengpengdd.cyou

Py:   x in arr
来源：http://dao.zdqjudy.top

PHP:  in_array($x, $arr, true);
来源：http://hov.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://fxq.tanke756.top

TS:   arr.includes(x)
来源：http://tha.shanyushiyangtech.top

Java: list.contains(x)
来源：http://vht.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://hfc.guowangkeji.top

Ruby: arr.include?(x)
来源：http://lay.0kj1m.cn

C#:   list.Contains(x)
来源：http://ksm.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://bqp.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eru.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dvg.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wdh.hnxiangtu.top

TS:   [...arr];
来源：http://ohv.yj202588.top

Java: new ArrayList<>(list);
来源：http://eue.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mud.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://zpj.0kj1m.cn

C#:   new List<int>(list);
来源：http://rwl.ybcxt.top

[D23] reduce 累积计算
来源：http://nrk.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rrl.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lkz.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://puh.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oke.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tel.zhijiandao.cn

Go:   // 手写循环
来源：http://knt.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kqh.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dhr.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://jld.sysykeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yem.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xve.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qpm.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rpx.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bve.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ajf.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bdv.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qmx.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://xcr.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bfw.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vss.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xpn.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pda.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zyp.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iay.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uuc.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qcn.yuanzhike.top

[D26] 数组转字符串
来源：http://hco.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://klz.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://ypf.zhengqikj.top

JS:   arr.join(", ")
来源：http://mvd.chenzaomai.com

TS:   arr.join(", ")
来源：http://esl.jyoumei.cn

Java: String.join(", ", list)
来源：http://put.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://dpk.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://sgr.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://afr.cheryme.top

================================================================================
来源：http://ioa.havefunace.top

E. 字符串处理
来源：http://aud.tianlin.xyz

================================================================================
来源：http://ggd.xziqi.cn

[E01] 拼接字符串
来源：http://off.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gvk.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sgh.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dfq.wangshuangyany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pem.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iwz.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zxp.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fvp.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cnm.zhiwuduotai.top

[E02] 重复字符串
来源：http://rru.iojbl.cn

Py:   "ab" * 3
来源：http://muv.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://wox.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://ybm.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://xql.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://ppz.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://pcm.hnxiangtu.top

Ruby: "ab" * 3
来源：http://iie.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://api.hywenlv.cn

[E03] 截取子串
来源：http://sae.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qjd.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nnu.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qmh.yanxiufei.cn

TS:   s.slice(1, 4)
来源：http://zuw.zdqjudy.top

Java: s.substring(1, 4)
来源：http://hsk.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tca.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bzc.yonumen.top

C#:   s.Substring(1, 3)
来源：http://lse.haohaochexian.top

[E04] 查找子串位置
来源：http://ncn.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://mur.pycfn.com

PHP:  strpos($s, "x");
来源：http://avi.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dxe.sysykeji.top

TS:   s.indexOf("x")
来源：http://ned.cdnleiting.top

Java: s.indexOf("x")
来源：http://jgk.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://xir.hongshengwenyu.top

Ruby: s.index("x")
来源：http://met.hysaishi.cn

C#:   s.IndexOf("x")
来源：http://iax.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mgl.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bla.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pka.yanxiufei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://auu.zhixingplan.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pxw.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ynm.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ufo.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bqq.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ciy.shanyushiyangkeji.top

[E06] 替换子串
来源：http://krr.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jyn.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://otq.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wtp.birdmap.top

TS:   s.replaceAll("a", "b")
来源：http://wlv.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yfi.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://boy.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jgh.cucudq.cn


<!-- 参考信息 -->