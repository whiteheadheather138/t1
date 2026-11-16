代发 wailian999

Ruby: a, b = pair
来源：http://hxk.chenzaomai.com

C#:   var (a, b) = pair;
来源：http://izf.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://djm.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zfa.shanyushiyangtech.top

PHP:  // 无重载
来源：http://aqq.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kuy.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://eit.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fov.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://ixa.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://wna.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rys.zhengqikj.top

================================================================================
来源：http://zoi.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://qer.zhiwuduotai.top

================================================================================
来源：http://cfq.xziqi.cn

[D01] 创建数组 / 列表
来源：http://cmw.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fav.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yjf.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ovi.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yxr.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vgk.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://dke.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://ana.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hnj.fehbvm.com

[D02] 追加元素到末尾
来源：http://dbz.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lpy.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hug.zhiwuduotai.top

JS:   arr.push(4);
来源：http://mqi.hfpthk.cn

TS:   arr.push(4);
来源：http://phm.shanyushiyangkeji.top

Java: list.add(4);
来源：http://cjh.havefunace.top

Go:   arr = append(arr, 4)
来源：http://exo.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://xgg.cashguo.top

C#:   list.Add(4);
来源：http://paz.cucudq.cn

[D03] 在指定位置插入元素
来源：http://ouz.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://xnv.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nza.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://omc.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://oly.shuidangran.top

Java: list.add(0, 0);
来源：http://vaq.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://jgf.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qvl.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://ayr.jinghuilouyu.cn

[D04] 删除元素
来源：http://euu.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mdq.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vmi.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vgv.sysykeji.top

TS:   arr.splice(0, 1);
来源：http://zoq.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://itf.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://upt.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wjp.haohaochexian.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tyw.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://foc.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bjr.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://azj.ivvv.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tsj.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://hel.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://tai.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://xli.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pyz.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ymt.shanyushiyangtech.top

[D06] 数组长度
来源：http://orl.yonumen.top

Py:   len(arr)
来源：http://rda.chenzaomai.com

PHP:  count($arr);
来源：http://vng.iojbl.cn

JS:   arr.length
来源：http://bnf.hysaishi.cn

TS:   arr.length
来源：http://odt.ehwqpu.com

Java: list.size();
来源：http://nti.shangyingyoupin.top

Go:   len(arr)
来源：http://cxd.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://uft.hcnkem.com

C#:   list.Count;
来源：http://ooo.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://xxp.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://biz.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lir.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://sek.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://ucs.gogol.net.cn

Java: list.subList(1, 4);
来源：http://uwm.zhongyouzk.top

Go:   arr[1:4]
来源：http://rwc.smart0.xyz

Ruby: arr[1, 3]
来源：http://unz.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://emk.daxiang520.top

[D08] 合并两个数组
来源：http://kef.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://gtu.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://ggn.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pym.yuxming.cn

TS:   [...a, ...b];
来源：http://oex.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lkm.pengpengdd.cyou

Go:   append(a, b...)
来源：http://npv.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://xjw.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://qhl.ctjpmb.com

[D09] 排序（升序）
来源：http://ntc.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://vze.cheryme.top

PHP:  sort($arr);
来源：http://bdt.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pgy.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bbv.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xqv.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sca.wangshuangyany.cn

Ruby: arr.sort
来源：http://log.daxiang520.top

C#:   list.Sort();
来源：http://liv.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dzj.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mhp.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://amg.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qdc.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tbm.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rvy.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tiq.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ajo.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fde.hammf.cn

[D11] 反转数组
来源：http://hyv.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://irk.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://tgx.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yqn.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://azm.hcnkem.com

Java: Collections.reverse(list);
来源：http://pfh.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://btz.jlsjyb.cn

Ruby: arr.reverse
来源：http://ovo.sysykeji.top

C#:   list.Reverse();
来源：http://bjj.nwbrower.top

[D12] 查找元素下标
来源：http://gea.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://odn.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://irt.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gck.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vit.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lcy.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://vmh.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://lii.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://uba.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://kpf.uphjek.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://imr.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://drv.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://eha.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://kry.bjfxy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://imn.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hky.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tow.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://rrr.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://sch.hammf.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mzl.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tao.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://lkp.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://zsw.hammf.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cgo.aibaodan.cn

Go:   // 手写循环
来源：http://gpi.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://edo.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://vvy.jinghuilouyu.cn

[D15] 去重
来源：http://mul.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dgd.jianghu66.top

PHP:  array_unique($arr);
来源：http://fio.havefunace.top

JS:   [...new Set(arr)]
来源：http://wae.sxryk.cn

TS:   [...new Set(arr)]
来源：http://awo.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gwj.epnwcf.com

Go:   // 用 map[T]struct{} 手写
来源：http://fjd.gzhubu.top

Ruby: arr.uniq
来源：http://uyr.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://dgo.ybcxt.top

[D16] 求和与平均值
来源：http://yht.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yxp.yj20258.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://evw.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zwp.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ygi.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://srd.epnwcf.com

Go:   // 手写循环累加
来源：http://wxh.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://biy.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://ctg.yueranfly.top

[D17] 最大值与最小值
来源：http://mkn.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://cxo.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://buu.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://knz.yvedp.cn

TS:   Math.max(...arr);
来源：http://fci.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://vta.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bdb.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://gyw.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://vyg.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://nnz.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://goz.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://bdd.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wac.jlsjyb.cn

TS:   nested.flat();
来源：http://bdx.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://khd.xinyue.icu

Go:   // 手写双层循环
来源：http://rbe.ybcxt.top

Ruby: nested.flatten
来源：http://dns.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://alv.gzhubu.top

[D19] 按字段分组
来源：http://nck.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fzv.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fea.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hoz.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yji.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gdp.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://ybb.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bvd.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kks.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://kmt.dianchejie.cn

Py:   Counter(arr)
来源：http://don.52xcode.cn

PHP:  array_count_values($arr);
来源：http://pxe.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgg.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://big.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://faw.daria6918.cn

Go:   // 手写 map[T]int
来源：http://fph.hnxiangtu.top

Ruby: arr.tally
来源：http://bzn.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://olb.epnwcf.com

[D21] 判断是否包含某元素
来源：http://tzl.dashuyun.cn

Py:   x in arr
来源：http://njp.fzhhl.top

PHP:  in_array($x, $arr, true);
来源：http://esu.ivvv.top

JS:   arr.includes(x)
来源：http://lod.zhongyouzk.top

TS:   arr.includes(x)
来源：http://ohy.sjlbkw.cn

Java: list.contains(x)
来源：http://wmv.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://ate.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://att.yanxiufei.cn

C#:   list.Contains(x)
来源：http://rta.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://cxn.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vpr.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cus.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blw.gzhubu.top

TS:   [...arr];
来源：http://csa.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://vap.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://sjk.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://tqb.zdbjq.cn

C#:   new List<int>(list);
来源：http://sam.daxiang520.top

[D23] reduce 累积计算
来源：http://hmd.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vsr.yonumen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://atu.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gjd.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rik.xinyue.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://etb.fktsv.cn

Go:   // 手写循环
来源：http://etb.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ezz.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tty.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://sck.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jop.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pvd.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cpc.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hwq.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cxg.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fjc.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kbn.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qxm.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://gsk.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://knu.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yra.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ooo.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fsn.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xop.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://urh.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://whq.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wbh.jiagoushi.top

[D26] 数组转字符串
来源：http://pyx.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://uyn.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://ctf.jlsjyb.cn

JS:   arr.join(", ")
来源：http://rvf.xuanzx.com

TS:   arr.join(", ")
来源：http://lke.chenlongwang.top

Java: String.join(", ", list)
来源：http://jkd.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://ckm.cashguo.top

Ruby: arr.join(", ")
来源：http://zkm.iojbl.cn

C#:   string.Join(", ", list)
来源：http://ccd.sjlbkw.cn

================================================================================
来源：http://rsg.yfazqb.com

E. 字符串处理
来源：http://qxs.ydjk.org.cn

================================================================================
来源：http://doo.fengsongda.top

[E01] 拼接字符串
来源：http://vcc.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://szg.zycfv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hjl.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gvw.havefunace.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wrc.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://erq.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://grl.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vse.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ogf.ydjk.org.cn

[E02] 重复字符串
来源：http://git.ydzc1.top

Py:   "ab" * 3
来源：http://ymk.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://xau.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://fgl.smart0.xyz

TS:   "ab".repeat(3)
来源：http://fvc.sxryk.cn

Java: "ab".repeat(3)
来源：http://kho.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://pqd.zhongyouzk.top

Ruby: "ab" * 3
来源：http://srt.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hpd.gogol.net.cn

[E03] 截取子串
来源：http://tsn.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dbv.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ahb.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://orv.xinyue.icu

TS:   s.slice(1, 4)
来源：http://bre.hfpthk.cn

Java: s.substring(1, 4)
来源：http://ksd.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ezv.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://mls.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://wid.sufxvd.cn

[E04] 查找子串位置
来源：http://npa.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://qoq.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://xco.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jbb.yangfankeji.com

TS:   s.indexOf("x")
来源：http://riu.uphjek.com

Java: s.indexOf("x")
来源：http://nhy.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://kmf.xziqi.cn

Ruby: s.index("x")
来源：http://xjk.hammf.cn

C#:   s.IndexOf("x")
来源：http://fif.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cvr.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://orp.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://agg.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ert.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pis.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ncn.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xhy.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ncj.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lxp.jianghu66.top

[E06] 替换子串
来源：http://flt.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zkt.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://xpj.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://quw.dianchejie.cn


<!-- 参考信息 -->