代发 wailian999

Ruby: a, b = pair
来源：http://iwv.yueranfly.top

C#:   var (a, b) = pair;
来源：http://pak.yj20258888.top

[C16] 函数 / 方法重载
来源：http://lef.shzxlz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vyc.gaohongyu789.top

PHP:  // 无重载
来源：http://zte.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ybs.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://mdp.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uds.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://exy.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://fud.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kvm.birdmap.top

================================================================================
来源：http://sif.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://rxp.sjlbkw.cn

================================================================================
来源：http://plo.sysykeji.top

[D01] 创建数组 / 列表
来源：http://ddy.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hfz.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dfe.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jpp.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lcb.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gzp.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://mcs.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://jcv.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iia.daxiang520.top

[D02] 追加元素到末尾
来源：http://wro.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pci.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jkf.jqgufenzy.top

JS:   arr.push(4);
来源：http://rnz.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://fjx.sxryk.cn

Java: list.add(4);
来源：http://zzv.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://ymf.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://ept.zdqjudy.top

C#:   list.Add(4);
来源：http://kgh.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://pjv.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://vhw.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fww.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://seo.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://zag.iojbl.cn

Java: list.add(0, 0);
来源：http://lfp.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://byc.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jip.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://eee.hesvh.cn

[D04] 删除元素
来源：http://mic.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ssp.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ugt.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dau.yongpay.top

TS:   arr.splice(0, 1);
来源：http://dxr.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vpr.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://edk.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://plx.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vpo.ehwqpu.com

[D05] 访问与修改元素
来源：http://gwr.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qdk.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qaj.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rot.guannengcc.top

TS:   arr[0]; arr.at(-1);
来源：http://era.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://sia.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://jvh.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zxq.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nef.chenlongwang.top

[D06] 数组长度
来源：http://pim.jinqigufen.top

Py:   len(arr)
来源：http://wyi.daxiang520.top

PHP:  count($arr);
来源：http://aea.hywenlv.cn

JS:   arr.length
来源：http://fqg.fktsv.cn

TS:   arr.length
来源：http://xcv.tanke756.top

Java: list.size();
来源：http://vpw.yuxming.cn

Go:   len(arr)
来源：http://mhs.yfazqb.com

Ruby: arr.length; arr.size
来源：http://evh.tanke756.top

C#:   list.Count;
来源：http://bpd.jianghu66.top

[D07] 切片 / 取子数组
来源：http://ksu.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gbk.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wrc.sjlbkw.cn

JS:   arr.slice(1, 4);
来源：http://pwb.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://pum.havefunace.top

Java: list.subList(1, 4);
来源：http://rag.zhoulong.xyz

Go:   arr[1:4]
来源：http://gzc.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://jqr.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://uqh.xinyue.icu

[D08] 合并两个数组
来源：http://frd.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://hfz.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://ozd.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://hrc.fengsongda.top

TS:   [...a, ...b];
来源：http://bbg.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qui.gaohongyu789.top

Go:   append(a, b...)
来源：http://pqr.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://uix.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://skd.zhiwuduotai.top

[D09] 排序（升序）
来源：http://ylt.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://car.zhiwuduotai.top

PHP:  sort($arr);
来源：http://lwi.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yqo.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dqm.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ahr.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qbs.hnxiangtu.top

Ruby: arr.sort
来源：http://gil.wangdashe.top

C#:   list.Sort();
来源：http://cpf.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://trx.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nsk.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bui.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://irr.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://urn.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qaq.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ppt.yonumen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://arh.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://adn.vqdsnc.cn

[D11] 反转数组
来源：http://cwy.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ees.birdmap.top

PHP:  array_reverse($arr);
来源：http://zyr.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rod.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://pya.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://abp.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://seg.yongpay.top

Ruby: arr.reverse
来源：http://eex.pengpengdd.cyou

C#:   list.Reverse();
来源：http://qyv.shzxlz.cn

[D12] 查找元素下标
来源：http://ksj.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://vnq.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pov.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mix.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bpp.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fai.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://dye.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://lsg.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://kpl.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://pvj.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uyp.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jdx.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://wtb.vqdsnc.cn

TS:   arr.filter(x => x > 3)
来源：http://mdt.yfazqb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hnv.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rld.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hyp.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bwr.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://fuq.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hcp.haohaochexian.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ade.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://llk.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://pmq.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ukw.fzhhl.top

Go:   // 手写循环
来源：http://dcq.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://wyc.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://drr.zhiwuduotai.top

[D15] 去重
来源：http://pio.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iem.jianghu66.top

PHP:  array_unique($arr);
来源：http://otd.jianghu66.top

JS:   [...new Set(arr)]
来源：http://xcq.jinqigfzy.top

TS:   [...new Set(arr)]
来源：http://ycl.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://acp.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://yzw.jiagoushi.top

Ruby: arr.uniq
来源：http://exs.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://eak.hnxiangtu.top

[D16] 求和与平均值
来源：http://cis.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://swf.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ycv.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://acc.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bdy.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qfd.sjlbkw.cn

Go:   // 手写循环累加
来源：http://mgp.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tsk.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://vfo.zhijiandao.cn

[D17] 最大值与最小值
来源：http://qyt.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://shw.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://kcy.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://von.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://izj.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xqj.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qnj.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://yff.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://abp.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://tgv.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lwf.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://qhq.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mal.birdmap.top

TS:   nested.flat();
来源：http://sdy.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://duz.vehdjk.com

Go:   // 手写双层循环
来源：http://ckz.fehbvm.com

Ruby: nested.flatten
来源：http://gyz.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://uja.wangshuangyany.cn

[D19] 按字段分组
来源：http://yqm.svipenyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gdg.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mzw.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nuq.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://woo.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aij.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://zqd.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://smn.guowangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nhw.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://wvv.havefunace.top

Py:   Counter(arr)
来源：http://kxm.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://gxh.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tsd.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nhh.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qnc.gzhubu.top

Go:   // 手写 map[T]int
来源：http://lve.shzxlz.cn

Ruby: arr.tally
来源：http://ysz.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://isa.52xcode.cn

[D21] 判断是否包含某元素
来源：http://evz.svipenyu.cn

Py:   x in arr
来源：http://xof.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://tcp.yj20258.top

JS:   arr.includes(x)
来源：http://zzi.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://zbq.yfazqb.com

Java: list.contains(x)
来源：http://joa.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://wah.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://znb.nwbrower.top

C#:   list.Contains(x)
来源：http://bqa.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://htl.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jwj.birdmap.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uco.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ewo.yvedp.cn

TS:   [...arr];
来源：http://xxi.52xcode.cn

Java: new ArrayList<>(list);
来源：http://idy.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://arq.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://nuu.aibaodan.cn

C#:   new List<int>(list);
来源：http://qws.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://tgk.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nae.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xvy.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://klm.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dnj.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xzp.gzhubu.top

Go:   // 手写循环
来源：http://shm.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://naj.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hwv.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://mjo.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tho.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gfh.jyoumei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bvo.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eqj.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dhw.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bia.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lte.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ifw.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://gbb.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xuw.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qnl.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://day.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tgl.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ltl.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aca.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gex.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cgi.yj20258.top

[D26] 数组转字符串
来源：http://uyg.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://zth.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://cpl.sxryk.cn

JS:   arr.join(", ")
来源：http://uyn.zhijiandao.cn

TS:   arr.join(", ")
来源：http://kuu.jinqigufen.top

Java: String.join(", ", list)
来源：http://zpw.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://tzi.guowangkeji.top

Ruby: arr.join(", ")
来源：http://dwo.sysykeji.top

C#:   string.Join(", ", list)
来源：http://lik.yonumen.top

================================================================================
来源：http://hgd.cashguo.top

E. 字符串处理
来源：http://rrf.daria6918.cn

================================================================================
来源：http://kik.ydjk.org.cn

[E01] 拼接字符串
来源：http://eoa.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pxs.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mjs.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gxa.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jbc.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dpt.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hyc.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tfr.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jxl.fengsongda.top

[E02] 重复字符串
来源：http://van.epnwcf.com

Py:   "ab" * 3
来源：http://xoo.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://max.316326.xyz

JS:   "ab".repeat(3)
来源：http://jnn.fktsv.cn

TS:   "ab".repeat(3)
来源：http://xiu.gzhubu.top

Java: "ab".repeat(3)
来源：http://bni.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://fjm.zhengqikj.top

Ruby: "ab" * 3
来源：http://dzo.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jty.gzhubu.top

[E03] 截取子串
来源：http://qps.havefunace.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kpk.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lvd.ybcxt.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qah.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://lxt.bjfxy.top

Java: s.substring(1, 4)
来源：http://wnk.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mzx.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://qiq.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://ujj.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://kwg.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://orw.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://tyr.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ctr.yuanzhike.top

TS:   s.indexOf("x")
来源：http://saa.yuanzhike.top

Java: s.indexOf("x")
来源：http://gij.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://mrz.fengsongda.top

Ruby: s.index("x")
来源：http://ucs.shuidangran.top

C#:   s.IndexOf("x")
来源：http://pxd.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ore.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fsx.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ecy.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://efz.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://zov.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bpz.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wlh.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hst.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lev.jinyuanbaomall.cn

[E06] 替换子串
来源：http://vkk.vqdsnc.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ben.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://ceo.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rbd.hnxiangtu.top


<!-- 参考信息 -->