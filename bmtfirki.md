代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eto.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sgy.zhixingplan.top

Java: // 无解构
来源：http://vdv.yfazqb.com

Go:   // 无解构
来源：http://ytt.gogol.net.cn

Ruby: a, b = pair
来源：http://pnp.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://cwd.hcnkem.com

[C16] 函数 / 方法重载
来源：http://arm.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://thu.zdqjudy.top

PHP:  // 无重载
来源：http://imi.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tdp.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://dbi.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lwr.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://ntf.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://igx.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gni.nanxinkj.top

================================================================================
来源：http://plh.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://uqj.aizwys.cn

================================================================================
来源：http://lxx.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://zxz.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xgt.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vws.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xgy.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://phw.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://npp.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://vmn.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://fcj.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nvs.guannengcc.top

[D02] 追加元素到末尾
来源：http://kbz.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jci.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lzc.ctjpmb.com

JS:   arr.push(4);
来源：http://qeo.52xcode.cn

TS:   arr.push(4);
来源：http://ica.tian-w.cn

Java: list.add(4);
来源：http://kce.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://qql.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://afm.zhiwuduotai.top

C#:   list.Add(4);
来源：http://gro.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://soo.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://qvg.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vwn.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vyv.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://lki.tarul.cn

Java: list.add(0, 0);
来源：http://fss.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://gjp.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://njg.uphjek.com

C#:   list.Insert(0, 0);
来源：http://rto.nanxinkj.top

[D04] 删除元素
来源：http://qsd.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kvl.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tef.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zlc.hammf.cn

TS:   arr.splice(0, 1);
来源：http://met.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vcg.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rnf.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mrj.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gpd.dianchejie.cn

[D05] 访问与修改元素
来源：http://ihd.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vxz.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pgi.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://umy.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://fyg.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://mmf.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://jnw.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rpg.jinghuilouyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ppc.vqdsnc.cn

[D06] 数组长度
来源：http://ruy.feifeiyinyue.top

Py:   len(arr)
来源：http://doc.kuanghao11.cn

PHP:  count($arr);
来源：http://qhz.hfpthk.cn

JS:   arr.length
来源：http://dus.cdnleiting.top

TS:   arr.length
来源：http://jst.hfpthk.cn

Java: list.size();
来源：http://swf.meibo888.top

Go:   len(arr)
来源：http://tto.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://lef.chenzaomai.com

C#:   list.Count;
来源：http://qle.ydzc1.top

[D07] 切片 / 取子数组
来源：http://gtr.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lzs.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://pyt.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://qdb.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://eqs.xylfe.cn

Java: list.subList(1, 4);
来源：http://zta.fehbvm.com

Go:   arr[1:4]
来源：http://jax.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://ecn.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://fuc.yangfankeji.com

[D08] 合并两个数组
来源：http://usr.sweek.top

Py:   a + b;  a.extend(b)
来源：http://ahz.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://mcb.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kxv.fktsv.cn

TS:   [...a, ...b];
来源：http://iiv.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fbr.daxiang520.top

Go:   append(a, b...)
来源：http://fwq.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://hjw.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://ztn.epnwcf.com

[D09] 排序（升序）
来源：http://ysw.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://kbv.chenjidiqi.icu

PHP:  sort($arr);
来源：http://hra.sufxvd.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://prk.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://njl.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bos.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qxa.zhijiandao.cn

Ruby: arr.sort
来源：http://ycj.xuetiantiany.cn

C#:   list.Sort();
来源：http://bfi.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ndw.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zhl.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fbu.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://twk.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cpd.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rnb.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dra.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ids.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tka.fzhhl.top

[D11] 反转数组
来源：http://fxh.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://qsg.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://hdo.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rhg.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://bor.yongpay.top

Java: Collections.reverse(list);
来源：http://muf.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://kel.guowangkeji.top

Ruby: arr.reverse
来源：http://jlh.jinqigufen.top

C#:   list.Reverse();
来源：http://ahp.hongshengwenyu.top

[D12] 查找元素下标
来源：http://tov.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://fnj.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zeo.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://etq.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nlc.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nlz.hammf.cn

Go:   slices.Index(arr, x)
来源：http://epq.yonumen.top

Ruby: arr.index(x)
来源：http://fpt.hcnkem.com

C#:   list.IndexOf(x);
来源：http://ioz.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://ccu.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kbj.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://thk.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://vqo.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://vtg.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lrb.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pbq.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mip.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://quu.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://ebo.xylfe.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xjp.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vid.ppjwa.cn

JS:   arr.map(x => x * 2)
来源：http://nfd.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://ilz.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://oxo.chenzaomai.com

Go:   // 手写循环
来源：http://qlz.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://lhx.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ota.zhongyouzk.top

[D15] 去重
来源：http://fbt.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://osq.gotoacloud.top

PHP:  array_unique($arr);
来源：http://jzv.hammf.cn

JS:   [...new Set(arr)]
来源：http://dbw.jinqigufen.top

TS:   [...new Set(arr)]
来源：http://piu.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dyv.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://ifq.sysykeji.top

Ruby: arr.uniq
来源：http://mjy.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://fby.nanxuanxn.top

[D16] 求和与平均值
来源：http://fcc.jqgfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fjb.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oom.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xjq.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wxe.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zve.52xcode.cn

Go:   // 手写循环累加
来源：http://xqe.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vif.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://aoh.yangfankeji.com

[D17] 最大值与最小值
来源：http://dbt.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://xho.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://orv.shuidangran.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eog.cashguo.top

TS:   Math.max(...arr);
来源：http://onf.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bfo.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nog.birdmap.top

Ruby: arr.max;  arr.min
来源：http://mtl.sysykeji.top

C#:   list.Max();  list.Min()
来源：http://gse.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://tzw.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ozg.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://ele.ctjpmb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kcm.hcnkem.com

TS:   nested.flat();
来源：http://fry.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dox.svipenyu.cn

Go:   // 手写双层循环
来源：http://htc.hongshengwenyu.top

Ruby: nested.flatten
来源：http://jtk.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://drw.aibaodan.cn

[D19] 按字段分组
来源：http://vjc.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mlg.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://svt.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vha.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://wqo.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://icl.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://irt.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ctf.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fsd.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://iby.guowangkeji.top

Py:   Counter(arr)
来源：http://edo.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://mak.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sco.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wmg.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cxp.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://lhh.ydzc1.top

Ruby: arr.tally
来源：http://jwx.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vtt.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://ybk.cucudq.cn

Py:   x in arr
来源：http://vdx.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://icu.dashuyun.cn

JS:   arr.includes(x)
来源：http://rem.sxryk.cn

TS:   arr.includes(x)
来源：http://pcg.uphjek.com

Java: list.contains(x)
来源：http://qgh.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://yim.jianghu66.top

Ruby: arr.include?(x)
来源：http://yxv.cucudq.cn

C#:   list.Contains(x)
来源：http://nwo.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://vao.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aht.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://syf.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bkt.jiagoushi.top

TS:   [...arr];
来源：http://etl.tanke756.top

Java: new ArrayList<>(list);
来源：http://ycw.gogol.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uuf.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://zum.ivvv.top

C#:   new List<int>(list);
来源：http://dfi.yueranfly.top

[D23] reduce 累积计算
来源：http://qyo.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zmt.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cxn.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ekr.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ryc.nanxinkj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nwq.nwbrower.top

Go:   // 手写循环
来源：http://qyu.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xtu.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zlf.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://pdl.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rdv.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fus.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ket.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jxn.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uea.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eup.sweek.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nmc.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kki.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://vkq.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xng.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ffs.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://djp.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cjg.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ghq.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://imf.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qaa.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ulh.cucudq.cn

[D26] 数组转字符串
来源：http://ddl.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://soy.yongpay.top

PHP:  implode(", ", $arr);
来源：http://icf.zhengqikj.top

JS:   arr.join(", ")
来源：http://vdc.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://sal.jyoumei.cn

Java: String.join(", ", list)
来源：http://gxi.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://rbp.yfazqb.com

Ruby: arr.join(", ")
来源：http://efz.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://fxi.cashguo.top

================================================================================
来源：http://yvu.ybcxt.top

E. 字符串处理
来源：http://fnt.hesvh.cn

================================================================================
来源：http://lcu.jianghu66.top

[E01] 拼接字符串
来源：http://paf.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eas.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://puh.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lpz.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ttg.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yer.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://phw.quarkkingdee.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dzl.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gcv.shangyingyoupin.top

[E02] 重复字符串
来源：http://jjx.gaohongyu789.top

Py:   "ab" * 3
来源：http://mkc.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://onz.fzhhl.top

JS:   "ab".repeat(3)
来源：http://bcp.daxiang520.top

TS:   "ab".repeat(3)
来源：http://aio.gogol.net.cn

Java: "ab".repeat(3)
来源：http://pea.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://qqo.tianlin.xyz

Ruby: "ab" * 3
来源：http://hfa.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zvv.zdbjq.cn

[E03] 截取子串
来源：http://tgz.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xmt.dashuyun.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vic.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qgn.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://yqf.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://kau.nanxinkj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tlx.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zcx.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://ooq.andypj.xyz

[E04] 查找子串位置
来源：http://ezd.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://wki.fzhhl.top

PHP:  strpos($s, "x");
来源：http://tvw.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://abw.yongpay.top

TS:   s.indexOf("x")
来源：http://pys.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://amh.yj202588.top

Go:   strings.Index(s, "x")
来源：http://adl.hnxiangtu.top

Ruby: s.index("x")
来源：http://idj.fktsv.cn

C#:   s.IndexOf("x")
来源：http://ygs.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xew.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mri.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yhl.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bso.fanxiaobao.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://rsb.svipenyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mkb.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://swk.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uqh.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://urh.shuidangran.top


<!-- 参考信息 -->