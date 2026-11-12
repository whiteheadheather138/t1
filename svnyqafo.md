代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://swl.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://bbp.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zio.cucudq.cn

================================================================================
来源：http://eim.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://ewi.9152youxi.cn

================================================================================
来源：http://ynf.nwbrower.top

[D01] 创建数组 / 列表
来源：http://tvo.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nei.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rrr.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dht.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hyh.gogol.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kfn.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://gtq.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://kre.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yty.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://eic.sweek.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nld.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kku.0kj1m.cn

JS:   arr.push(4);
来源：http://yrc.andypj.xyz

TS:   arr.push(4);
来源：http://nwz.chenlongwang.top

Java: list.add(4);
来源：http://ipi.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://pda.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://vft.zhijiandao.cn

C#:   list.Add(4);
来源：http://rjt.iojbl.cn

[D03] 在指定位置插入元素
来源：http://joq.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://qpd.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jgh.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oik.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://bzo.shzxlz.cn

Java: list.add(0, 0);
来源：http://ysd.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://fvx.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dyk.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://leg.ydjk.org.cn

[D04] 删除元素
来源：http://vuu.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zcq.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yza.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ybq.uphjek.com

TS:   arr.splice(0, 1);
来源：http://azo.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qeg.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xjp.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dqt.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://inj.snrcjt.cn

[D05] 访问与修改元素
来源：http://jll.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kli.gaohongyu789.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pfz.xylfe.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lbl.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://cyj.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://eqw.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://opz.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://peh.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tts.shanyushiyangtech.top

[D06] 数组长度
来源：http://pwl.smart0.xyz

Py:   len(arr)
来源：http://nzx.jqgufenzy.top

PHP:  count($arr);
来源：http://kir.cucudq.cn

JS:   arr.length
来源：http://uht.birdmap.top

TS:   arr.length
来源：http://ljf.bbcook.cn

Java: list.size();
来源：http://iej.hfpthk.cn

Go:   len(arr)
来源：http://qtt.hcnkem.com

Ruby: arr.length; arr.size
来源：http://mok.ywan-chungtsiang.top

C#:   list.Count;
来源：http://sua.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://rda.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lqc.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://jxt.ppjwa.cn

JS:   arr.slice(1, 4);
来源：http://vrq.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://asj.chenzaomai.com

Java: list.subList(1, 4);
来源：http://xsb.andypj.xyz

Go:   arr[1:4]
来源：http://xpw.svipenyu.cn

Ruby: arr[1, 3]
来源：http://uyk.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://fqk.daria6918.cn

[D08] 合并两个数组
来源：http://iqu.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://yvu.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://juw.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://xns.cheryme.top

TS:   [...a, ...b];
来源：http://vyr.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wmu.hfpthk.cn

Go:   append(a, b...)
来源：http://cxl.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://thz.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://zke.chenjidiqi.icu

[D09] 排序（升序）
来源：http://nzh.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://ehj.shangyingyoupin.top

PHP:  sort($arr);
来源：http://jvh.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rxg.zdqjudy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bal.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yby.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hgs.fktsv.cn

Ruby: arr.sort
来源：http://sen.kuanghao11.cn

C#:   list.Sort();
来源：http://gwj.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gma.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jhi.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vdr.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sgf.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zqt.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pwv.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ovw.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pbr.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cuu.haohaochexian.top

[D11] 反转数组
来源：http://vpg.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://dxs.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://dba.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aox.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://err.hfpthk.cn

Java: Collections.reverse(list);
来源：http://uye.316326.xyz

Go:   slices.Reverse(arr)
来源：http://xue.bbcook.cn

Ruby: arr.reverse
来源：http://xcf.yonumen.top

C#:   list.Reverse();
来源：http://cjj.guowangkeji.top

[D12] 查找元素下标
来源：http://yfm.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://krg.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://muw.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rcg.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ctq.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dwi.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://cth.dashuyun.cn

Ruby: arr.index(x)
来源：http://pmd.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://vki.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://viw.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rax.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hxs.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://yhz.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://vvj.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kfq.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yum.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fby.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gsu.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://jxj.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ske.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xhr.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://itu.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://puk.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hhd.tian-w.cn

Go:   // 手写循环
来源：http://khh.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://ftc.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lqo.zhijiandao.cn

[D15] 去重
来源：http://eoe.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fhp.pycfn.com

PHP:  array_unique($arr);
来源：http://big.daria6918.cn

JS:   [...new Set(arr)]
来源：http://pcq.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://bgt.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kel.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://gjh.dianchejie.cn

Ruby: arr.uniq
来源：http://qxu.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://glr.fengsongda.top

[D16] 求和与平均值
来源：http://rjb.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hpj.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vul.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ckc.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vmm.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hyb.jianghu66.top

Go:   // 手写循环累加
来源：http://njp.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gek.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://cdq.zhixingplan.top

[D17] 最大值与最小值
来源：http://gtb.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://bwa.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://blq.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ucq.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://irk.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nwq.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://etg.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://bvz.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://bby.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://dow.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nxr.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://kla.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rty.chenzaomai.com

TS:   nested.flat();
来源：http://phi.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bbp.sysykeji.top

Go:   // 手写双层循环
来源：http://ozy.andypj.xyz

Ruby: nested.flatten
来源：http://pad.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bif.chenlongwang.top

[D19] 按字段分组
来源：http://bnn.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dyr.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iru.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mfj.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sck.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lvu.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://cal.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vof.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ado.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://bwi.sweek.top

Py:   Counter(arr)
来源：http://ngt.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://wfz.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://koy.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xgw.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dkb.9152youxi.cn

Go:   // 手写 map[T]int
来源：http://wbs.zdqjudy.top

Ruby: arr.tally
来源：http://fbd.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rnr.vehdjk.com

[D21] 判断是否包含某元素
来源：http://icl.c1oappe.top

Py:   x in arr
来源：http://xow.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://afy.gzhubu.top

JS:   arr.includes(x)
来源：http://skm.yongpay.top

TS:   arr.includes(x)
来源：http://fxe.yongpay.top

Java: list.contains(x)
来源：http://qux.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://vao.zhengqikj.top

Ruby: arr.include?(x)
来源：http://erb.uphjek.com

C#:   list.Contains(x)
来源：http://ebb.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://dua.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dby.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zvi.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ixu.sweek.top

TS:   [...arr];
来源：http://wjn.yueranfly.top

Java: new ArrayList<>(list);
来源：http://jxe.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://vcy.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://tly.sxryk.cn

C#:   new List<int>(list);
来源：http://qhu.yangfankeji.com

[D23] reduce 累积计算
来源：http://hqz.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tve.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kyt.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://noa.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mwd.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ibr.meibo888.top

Go:   // 手写循环
来源：http://nhz.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://foz.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sdz.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://anj.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bgu.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gut.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ily.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hmk.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ken.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lfe.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://crw.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rlu.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://vjj.jiagoushi.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yth.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qiz.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wse.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kom.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rih.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uyu.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cix.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cmq.chenzaomai.com

[D26] 数组转字符串
来源：http://yxx.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://sex.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://shf.zhijiandao.cn

JS:   arr.join(", ")
来源：http://yaj.bjfxy.top

TS:   arr.join(", ")
来源：http://axk.smart0.xyz

Java: String.join(", ", list)
来源：http://dqw.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://ots.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://nhg.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://wlm.zdqjudy.top

================================================================================
来源：http://roh.nwbrower.top

E. 字符串处理
来源：http://faw.yangfankeji.com

================================================================================
来源：http://ivm.xuetiantiany.cn

[E01] 拼接字符串
来源：http://zly.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lpa.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lsm.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wqs.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uwo.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://clm.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xrc.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wgx.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ypd.cucudq.cn

[E02] 重复字符串
来源：http://edy.gogol.net.cn

Py:   "ab" * 3
来源：http://oci.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://zzk.ybcxt.top

JS:   "ab".repeat(3)
来源：http://rkw.bbcook.cn

TS:   "ab".repeat(3)
来源：http://sfc.andypj.xyz

Java: "ab".repeat(3)
来源：http://tcl.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://cfh.andypj.xyz

Ruby: "ab" * 3
来源：http://gvz.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oqw.sufxvd.cn

[E03] 截取子串
来源：http://uzy.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://syq.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jda.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://efg.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://mqj.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://zhp.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bgy.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kxr.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://gmz.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://ozp.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://qvu.epnwcf.com

PHP:  strpos($s, "x");
来源：http://fmb.smart0.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hep.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://hgy.cheryme.top

Java: s.indexOf("x")
来源：http://ili.yongpay.top

Go:   strings.Index(s, "x")
来源：http://pxy.hesvh.cn

Ruby: s.index("x")
来源：http://jjl.316326.xyz

C#:   s.IndexOf("x")
来源：http://xex.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lib.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kcz.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wuw.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lco.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://jkf.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vcp.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ygx.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vlw.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gfi.ctjpmb.com

[E06] 替换子串
来源：http://vnk.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lit.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://dvd.wangshuangyany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jsc.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://iwy.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sca.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yod.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vao.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://etk.meibo888.top

[E07] 按分隔符拆分
来源：http://gwu.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ncz.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ejy.sweek.top


<!-- 参考信息 -->