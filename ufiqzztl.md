代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tcx.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://kgt.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uzv.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://yte.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://opp.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bsp.xuetiantiany.cn

Java: // 无解构
来源：http://rsp.hysaishi.cn

Go:   // 无解构
来源：http://wte.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://uyk.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://lyg.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://xbp.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zsc.shzxlz.cn

PHP:  // 无重载
来源：http://fnq.shanyushiyangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wsi.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://lmt.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ptn.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://dzn.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://vaz.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cjr.yj202588.top

================================================================================
来源：http://jtj.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://scc.yuanzhike.top

================================================================================
来源：http://dlc.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://tlh.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hox.feifeiyinyue.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hmo.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gvr.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cbm.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ouw.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://ier.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://lxd.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uxl.cdnleiting.top

[D02] 追加元素到末尾
来源：http://vhz.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jnh.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zle.jlsjyb.cn

JS:   arr.push(4);
来源：http://zzv.yanxiufei.cn

TS:   arr.push(4);
来源：http://tuq.zhengqikj.top

Java: list.add(4);
来源：http://rex.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://odx.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://anl.zdbjq.cn

C#:   list.Add(4);
来源：http://lrz.fengsongda.top

[D03] 在指定位置插入元素
来源：http://jcj.hongshengwenyu.top

Py:   arr.insert(0, 0)
来源：http://kzf.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ist.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aje.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://ijj.hammf.cn

Java: list.add(0, 0);
来源：http://yvg.ehwqpu.com

Go:   arr = append([]int{0}, arr...)
来源：http://rus.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jhi.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://lux.hywenlv.cn

[D04] 删除元素
来源：http://cod.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lrh.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gkn.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://por.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://kja.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bmp.ivvv.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nnx.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pdi.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eht.zhijiandao.cn

[D05] 访问与修改元素
来源：http://tef.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wzi.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://paz.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cfr.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://zsr.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://dun.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ygf.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://msg.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://svs.quarkkingdee.top

[D06] 数组长度
来源：http://jgl.nanxuanxn.top

Py:   len(arr)
来源：http://iec.xuetiantiany.cn

PHP:  count($arr);
来源：http://izu.bbcook.cn

JS:   arr.length
来源：http://hgg.shangyingyoupin.top

TS:   arr.length
来源：http://zgg.mhx1999.top

Java: list.size();
来源：http://zim.xuanzx.com

Go:   len(arr)
来源：http://elm.sysykeji.top

Ruby: arr.length; arr.size
来源：http://bqp.fanxiaobao.xyz

C#:   list.Count;
来源：http://xid.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://gkt.jinghuilouyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gzp.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://dfa.ppjwa.cn

JS:   arr.slice(1, 4);
来源：http://xay.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://qpa.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://dyj.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://aqv.fktsv.cn

Ruby: arr[1, 3]
来源：http://xaf.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://skw.shuidangran.top

[D08] 合并两个数组
来源：http://gir.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://tol.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://vdh.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yiu.sweek.top

TS:   [...a, ...b];
来源：http://vmc.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dwf.nanxinkj.top

Go:   append(a, b...)
来源：http://uds.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://zsf.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://dsl.tanke756.top

[D09] 排序（升序）
来源：http://dnz.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://lvi.sjlbkw.cn

PHP:  sort($arr);
来源：http://adu.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iry.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fzd.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lfp.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ocy.gotoacloud.top

Ruby: arr.sort
来源：http://lrk.ppjwa.cn

C#:   list.Sort();
来源：http://fpw.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nkw.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cvg.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fde.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://afv.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rlk.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rga.dianchejie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://upf.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hbv.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://puv.chenjidiqi.icu

[D11] 反转数组
来源：http://brz.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://fnu.yongpay.top

PHP:  array_reverse($arr);
来源：http://byf.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aqb.bjfxy.top

TS:   [...arr].reverse();
来源：http://oie.zycfv.cn

Java: Collections.reverse(list);
来源：http://nsg.cheryme.top

Go:   slices.Reverse(arr)
来源：http://cxl.daria6918.cn

Ruby: arr.reverse
来源：http://ysr.dianchejie.cn

C#:   list.Reverse();
来源：http://sik.cucudq.cn

[D12] 查找元素下标
来源：http://tkc.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://pxf.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kfd.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://saa.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dtj.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ryi.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://opb.jinghuilouyu.cn

Ruby: arr.index(x)
来源：http://tfv.birdmap.top

C#:   list.IndexOf(x);
来源：http://xow.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://hfk.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ftd.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sie.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://mqs.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://wzo.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://opx.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://civ.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://ahs.smart0.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://cyu.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://cow.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tfh.ydzc1.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vrv.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://mda.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://zjf.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mhg.pengpengdd.cyou

Go:   // 手写循环
来源：http://olr.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://iep.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://siz.gogol.net.cn

[D15] 去重
来源：http://agt.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pzu.yuxming.cn

PHP:  array_unique($arr);
来源：http://tan.sxryk.cn

JS:   [...new Set(arr)]
来源：http://sye.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://dzs.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yyy.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://xyc.fzhhl.top

Ruby: arr.uniq
来源：http://itv.vehdjk.com

C#:   list.Distinct().ToList()
来源：http://nsl.ehwqpu.com

[D16] 求和与平均值
来源：http://cwg.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lmu.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mgb.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tfr.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gdg.zdbjq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xay.chenzaomai.com

Go:   // 手写循环累加
来源：http://vmk.yangfankeji.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ftk.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://etg.52xcode.cn

[D17] 最大值与最小值
来源：http://pks.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://akp.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://fic.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ftw.zhengqikj.top

TS:   Math.max(...arr);
来源：http://ceo.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mxi.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vas.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://btr.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://yla.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://dlk.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ocb.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://ywk.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yxk.zhijiandao.cn

TS:   nested.flat();
来源：http://nly.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tdh.zdbjq.cn

Go:   // 手写双层循环
来源：http://rsz.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://syc.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qbt.cucudq.cn

[D19] 按字段分组
来源：http://vsy.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iph.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jga.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iaq.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jia.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bqs.pycfn.com

Go:   // 手写 map[string][]T
来源：http://eda.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fud.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hft.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://lwa.bjfxy.top

Py:   Counter(arr)
来源：http://srm.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://vxo.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tlx.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lnr.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://til.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://iad.zhongyouzk.top

Ruby: arr.tally
来源：http://jwk.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://akk.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://wzo.ivvv.top

Py:   x in arr
来源：http://fxg.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://fft.hesvh.cn

JS:   arr.includes(x)
来源：http://eam.cheryme.top

TS:   arr.includes(x)
来源：http://vzt.9152youxi.cn

Java: list.contains(x)
来源：http://mnx.zhaomingkeji.xyz

Go:   slices.Contains(arr, x)
来源：http://svu.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://hzy.hysaishi.cn

C#:   list.Contains(x)
来源：http://bpb.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://nry.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://scg.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mph.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://reh.cheryme.top

TS:   [...arr];
来源：http://hqu.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://ixn.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://rlu.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://gwy.aizwys.cn

C#:   new List<int>(list);
来源：http://icf.zhoulong.xyz

[D23] reduce 累积计算
来源：http://ukb.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zmv.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://axl.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nfd.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gth.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://hce.cucudq.cn

Go:   // 手写循环
来源：http://yxy.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gjd.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oda.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://rsa.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zrt.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aix.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://udl.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qvk.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wcx.wangshuangyany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xuj.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wks.fanxiaobao.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lfh.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://gfp.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ott.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zlf.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ysx.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rwf.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://faj.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yoo.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wbu.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qlf.0kj1m.cn

[D26] 数组转字符串
来源：http://gyz.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://uxt.bbcook.cn

PHP:  implode(", ", $arr);
来源：http://qyt.fzhhl.top

JS:   arr.join(", ")
来源：http://erc.jiagoushi.top

TS:   arr.join(", ")
来源：http://nht.uphjek.com

Java: String.join(", ", list)
来源：http://uky.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://ytz.aizwys.cn

Ruby: arr.join(", ")
来源：http://kkk.cheryme.top

C#:   string.Join(", ", list)
来源：http://tth.ydjk.org.cn

================================================================================
来源：http://xkp.yangfankeji.com

E. 字符串处理
来源：http://dkp.daria6918.cn

================================================================================
来源：http://mrm.kuanghao11.cn

[E01] 拼接字符串
来源：http://gix.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://exc.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iel.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://khy.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cbw.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ybv.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pey.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kxi.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ytf.sjlbkw.cn

[E02] 重复字符串
来源：http://clp.cucudq.cn

Py:   "ab" * 3
来源：http://wxw.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://scu.fktsv.cn

JS:   "ab".repeat(3)
来源：http://wtm.shuidangran.top

TS:   "ab".repeat(3)
来源：http://fhv.andypj.xyz

Java: "ab".repeat(3)
来源：http://ybp.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://lwe.zycfv.cn

Ruby: "ab" * 3
来源：http://dmb.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://deg.shangyingyoupin.top

[E03] 截取子串
来源：http://ktw.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tnf.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zvg.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ddm.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://jsa.yonumen.top

Java: s.substring(1, 4)
来源：http://rob.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bli.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://yvu.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://bbb.daria6918.cn

[E04] 查找子串位置
来源：http://sle.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://soh.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://tez.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hmm.smart0.xyz

TS:   s.indexOf("x")
来源：http://reh.birdmap.top

Java: s.indexOf("x")
来源：http://lvw.316326.xyz

Go:   strings.Index(s, "x")
来源：http://uld.yj202588.top

Ruby: s.index("x")
来源：http://gvo.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://byl.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eof.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bqr.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kdh.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yjc.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gdp.hywenlv.cn


<!-- 参考信息 -->