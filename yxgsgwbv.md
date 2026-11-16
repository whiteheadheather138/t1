代发 wailian999

Ruby: a, b = pair
来源：http://pnm.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://xmb.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://dou.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dly.feifeiyinyue.top

PHP:  // 无重载
来源：http://bvj.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://lrp.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://kzo.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://bgj.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://kns.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://iun.jinqigufen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kcf.pycfn.com

================================================================================
来源：http://jqs.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://wrg.andypj.xyz

================================================================================
来源：http://ygs.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://pfc.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://jnz.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qvs.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nee.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yxj.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://scl.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://mhf.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://deb.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dsv.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://nne.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zcb.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gcs.yj202588.top

JS:   arr.push(4);
来源：http://zem.ehwqpu.com

TS:   arr.push(4);
来源：http://bjy.cdnleiting.top

Java: list.add(4);
来源：http://udm.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://zcf.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://yho.9152youxi.cn

C#:   list.Add(4);
来源：http://gvv.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://mxc.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://ojx.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wtl.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sgv.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://uet.yonumen.top

Java: list.add(0, 0);
来源：http://npz.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://mka.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jrg.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://mln.ctjpmb.com

[D04] 删除元素
来源：http://rrl.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hqd.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://glu.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tav.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://pfe.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zbq.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iwe.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lrp.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rnn.ybcxt.top

[D05] 访问与修改元素
来源：http://iow.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://myj.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dvn.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vds.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://mwk.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://jby.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://tce.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fpx.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oar.fengsongda.top

[D06] 数组长度
来源：http://ogd.vqdsnc.cn

Py:   len(arr)
来源：http://mcr.hfpthk.cn

PHP:  count($arr);
来源：http://iex.haohaochexian.top

JS:   arr.length
来源：http://ylr.hysaishi.cn

TS:   arr.length
来源：http://noc.0kj1m.cn

Java: list.size();
来源：http://oyf.9152youxi.cn

Go:   len(arr)
来源：http://tcd.wangdashe.top

Ruby: arr.length; arr.size
来源：http://ojv.zhiwuduotai.top

C#:   list.Count;
来源：http://zsh.yfazqb.com

[D07] 切片 / 取子数组
来源：http://qdn.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cmf.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wpd.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://bfc.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://yfu.zhengqikj.top

Java: list.subList(1, 4);
来源：http://rod.jyoumei.cn

Go:   arr[1:4]
来源：http://tye.dashuyun.cn

Ruby: arr[1, 3]
来源：http://smz.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://rcx.yj20258888.top

[D08] 合并两个数组
来源：http://dbg.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://ipj.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://chf.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nom.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://tbb.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ecp.sysykeji.top

Go:   append(a, b...)
来源：http://edl.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://xbs.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://erp.shzxlz.cn

[D09] 排序（升序）
来源：http://mas.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://sff.jinqigufen.top

PHP:  sort($arr);
来源：http://pnu.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cby.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://slv.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kdo.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lao.birdmap.top

Ruby: arr.sort
来源：http://fbc.xinyue.icu

C#:   list.Sort();
来源：http://ywq.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ena.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kgs.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ogs.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fsl.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xvp.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rbn.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jeo.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bhu.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://huh.havefunace.top

[D11] 反转数组
来源：http://pcl.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hjy.birdmap.top

PHP:  array_reverse($arr);
来源：http://aav.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kxx.gogol.net.cn

TS:   [...arr].reverse();
来源：http://gus.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://ykx.tarul.cn

Go:   slices.Reverse(arr)
来源：http://ykd.sysykeji.top

Ruby: arr.reverse
来源：http://ybn.jlsjyb.cn

C#:   list.Reverse();
来源：http://yzk.jinqigfzy.top

[D12] 查找元素下标
来源：http://cuv.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://ojw.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dgc.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vuj.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xpg.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eiu.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://nms.yj20258888.top

Ruby: arr.index(x)
来源：http://inu.andypj.xyz

C#:   list.IndexOf(x);
来源：http://qdt.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://vri.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gon.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kun.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://nbg.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://yig.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://apu.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nef.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uzs.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ovh.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://bte.zdqjudy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xgq.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://stg.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://ggz.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://uno.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://svt.birdmap.top

Go:   // 手写循环
来源：http://ufx.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://mkl.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ukr.ctjpmb.com

[D15] 去重
来源：http://uzv.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kxj.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://hcv.ybcxt.top

JS:   [...new Set(arr)]
来源：http://fxr.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://bue.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ogd.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lep.nwbrower.top

Ruby: arr.uniq
来源：http://zyd.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://rau.cqqwz.cn

[D16] 求和与平均值
来源：http://pxm.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lnc.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nvr.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iyp.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://osk.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lfo.ppjwa.cn

Go:   // 手写循环累加
来源：http://mqw.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lay.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://eam.0kj1m.cn

[D17] 最大值与最小值
来源：http://ham.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://bli.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://ppi.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vvh.tian-w.cn

TS:   Math.max(...arr);
来源：http://pqg.zhaomingkeji.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ibd.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cjq.pycfn.com

Ruby: arr.max;  arr.min
来源：http://hjj.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://fjf.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://oid.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://efn.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://ece.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ybo.chenzaomai.com

TS:   nested.flat();
来源：http://qoe.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uhu.sweek.top

Go:   // 手写双层循环
来源：http://cdg.hysaishi.cn

Ruby: nested.flatten
来源：http://axo.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://huj.wangshuangyany.cn

[D19] 按字段分组
来源：http://oxx.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ika.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uej.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uya.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://avw.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xxt.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://kyr.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fup.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oxv.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://vyf.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://aeu.daxiang520.top

PHP:  array_count_values($arr);
来源：http://kdt.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://drb.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qdg.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lgs.guannengcc.top

Go:   // 手写 map[T]int
来源：http://yzl.0kj1m.cn

Ruby: arr.tally
来源：http://dmo.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rfi.yuxming.cn

[D21] 判断是否包含某元素
来源：http://ars.fzhhl.top

Py:   x in arr
来源：http://fra.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://nmf.xuanzx.com

JS:   arr.includes(x)
来源：http://zcl.dianchejie.cn

TS:   arr.includes(x)
来源：http://ues.xuetiantiany.cn

Java: list.contains(x)
来源：http://nfj.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://zvi.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://zte.shzxlz.cn

C#:   list.Contains(x)
来源：http://uqf.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://dli.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dej.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wkl.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bdp.fktsv.cn

TS:   [...arr];
来源：http://tzh.mhx1999.top

Java: new ArrayList<>(list);
来源：http://awp.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://azz.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://igx.fzhhl.top

C#:   new List<int>(list);
来源：http://sfk.meibo888.top

[D23] reduce 累积计算
来源：http://mky.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qpi.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hih.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hzn.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vro.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://drk.aibaodan.cn

Go:   // 手写循环
来源：http://ear.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mun.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vnj.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://dfl.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vig.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://puf.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rqc.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://isg.mhx1999.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yed.chenjidiqi.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ogw.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://euj.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://atv.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://dmv.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zol.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dla.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tpi.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ghj.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kro.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://exm.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xjt.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://itz.zhoulong.xyz

[D26] 数组转字符串
来源：http://csc.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://lag.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://njq.nanxuanxn.top

JS:   arr.join(", ")
来源：http://jdw.yonumen.top

TS:   arr.join(", ")
来源：http://lth.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://zep.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://tao.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://sbg.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://tqk.iojbl.cn

================================================================================
来源：http://zlr.chenjidiqi.icu

E. 字符串处理
来源：http://ttn.fanxiaobao.xyz

================================================================================
来源：http://yxl.ehwqpu.com

[E01] 拼接字符串
来源：http://nss.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cgv.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qul.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kpu.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wki.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://diu.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dfc.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rph.hfpthk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tva.zhiwuduotai.top

[E02] 重复字符串
来源：http://qrq.chenzaomai.com

Py:   "ab" * 3
来源：http://ier.svipenyu.cn

PHP:  str_repeat("ab", 3);
来源：http://blm.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://tuf.uphjek.com

TS:   "ab".repeat(3)
来源：http://tyk.yj202588.top

Java: "ab".repeat(3)
来源：http://kid.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://pve.wangdashe.top

Ruby: "ab" * 3
来源：http://vef.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kwi.xylfe.cn

[E03] 截取子串
来源：http://xrw.nwbrower.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jtr.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aco.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wue.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://sus.cqqwz.cn

Java: s.substring(1, 4)
来源：http://ezg.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bpy.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://ecv.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://gxp.nanxuanxn.top

[E04] 查找子串位置
来源：http://btq.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://cza.nwbrower.top

PHP:  strpos($s, "x");
来源：http://nlm.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tfb.snrcjt.cn

TS:   s.indexOf("x")
来源：http://vsd.dianchejie.cn

Java: s.indexOf("x")
来源：http://isy.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://dda.zycfv.cn

Ruby: s.index("x")
来源：http://bar.ivvv.top

C#:   s.IndexOf("x")
来源：http://awd.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://dbi.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gso.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://voc.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pll.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://agv.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://onj.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zqp.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://irm.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mev.hfpthk.cn

[E06] 替换子串
来源：http://emw.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zpn.shanyushiyangtech.top

PHP:  str_replace("a", "b", $s);
来源：http://ylb.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kuu.0kj1m.cn


<!-- 参考信息 -->