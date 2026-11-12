代发 wailian999

PHP:  // 无重载
来源：http://txw.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://gjn.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://myh.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://axg.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://bxu.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://hrg.yj20258.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ens.havefunace.top

================================================================================
来源：http://ykv.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://ule.fanxiaobao.xyz

================================================================================
来源：http://ifa.sxryk.cn

[D01] 创建数组 / 列表
来源：http://wxl.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://dji.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://roq.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ipd.wangshuangyany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ohg.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ikr.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://zjn.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://kvf.dianchejie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wfl.cheryme.top

[D02] 追加元素到末尾
来源：http://sct.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iuh.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gks.bjfxy.top

JS:   arr.push(4);
来源：http://lud.guannengcc.top

TS:   arr.push(4);
来源：http://juw.jinyuanbaomall.cn

Java: list.add(4);
来源：http://mpt.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://ixh.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://gze.cashguo.top

C#:   list.Add(4);
来源：http://yqg.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://qpr.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://dqn.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qid.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yzg.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://tda.ehwqpu.com

Java: list.add(0, 0);
来源：http://sbb.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xfo.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cgh.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://pwo.zdqjudy.top

[D04] 删除元素
来源：http://xpl.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ces.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ptc.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aug.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://plt.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uzm.zhijiandao.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wsr.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://adb.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yst.jqgufenzy.top

[D05] 访问与修改元素
来源：http://top.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://igm.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wsi.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uhs.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://fau.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://ccs.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://vlk.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ezu.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vdz.cucudq.cn

[D06] 数组长度
来源：http://vkl.daxiang520.top

Py:   len(arr)
来源：http://tha.shuidangran.top

PHP:  count($arr);
来源：http://soh.hnqzz.top

JS:   arr.length
来源：http://tyj.hesvh.cn

TS:   arr.length
来源：http://mze.kuanghao11.cn

Java: list.size();
来源：http://rgf.smart0.xyz

Go:   len(arr)
来源：http://spt.xuanzx.com

Ruby: arr.length; arr.size
来源：http://rtx.yonumen.top

C#:   list.Count;
来源：http://mme.xylfe.cn

[D07] 切片 / 取子数组
来源：http://yne.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mfu.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://icc.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://azu.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://mvi.aibaodan.cn

Java: list.subList(1, 4);
来源：http://xmb.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://jjz.nanxinkj.top

Ruby: arr[1, 3]
来源：http://sew.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://aii.hywenlv.cn

[D08] 合并两个数组
来源：http://wsz.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://pkp.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://vqj.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nkc.dianchejie.cn

TS:   [...a, ...b];
来源：http://fic.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xax.52xcode.cn

Go:   append(a, b...)
来源：http://ahq.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://joh.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://zii.chenjidiqi.icu

[D09] 排序（升序）
来源：http://pyv.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://fjc.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://csy.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rcp.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://arw.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fcj.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vcq.pycfn.com

Ruby: arr.sort
来源：http://tpz.tianlin.xyz

C#:   list.Sort();
来源：http://uyi.sjlbkw.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ind.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ror.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xro.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sdv.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pfn.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zgw.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dyj.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zyx.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iel.xuanzx.com

[D11] 反转数组
来源：http://myp.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://zfa.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://jfq.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bow.yj202588.top

TS:   [...arr].reverse();
来源：http://oqb.snrcjt.cn

Java: Collections.reverse(list);
来源：http://vex.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://jyr.nanxinkj.top

Ruby: arr.reverse
来源：http://iup.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://vrb.fengsongda.top

[D12] 查找元素下标
来源：http://ckp.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://wkq.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lgj.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehg.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gvs.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mgo.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://ate.gzhubu.top

Ruby: arr.index(x)
来源：http://xoo.havefunace.top

C#:   list.IndexOf(x);
来源：http://pde.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://sur.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ggj.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kut.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://blv.yj202588.top

TS:   arr.filter(x => x > 3)
来源：http://dmk.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fom.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ara.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://cwl.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://jno.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://ncl.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ocz.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xxn.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://qfq.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://jwi.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dxo.tanke756.top

Go:   // 手写循环
来源：http://glq.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nie.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tnz.xingfuxueyuan.xyz

[D15] 去重
来源：http://bem.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lrc.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://qfl.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://xbs.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://tgc.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zjl.chenlongwang.top

Go:   // 用 map[T]struct{} 手写
来源：http://gpx.wangshuangyany.cn

Ruby: arr.uniq
来源：http://mim.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://ozu.zhongyouzk.top

[D16] 求和与平均值
来源：http://rjt.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aur.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://szd.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://luz.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jzl.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bqz.pycfn.com

Go:   // 手写循环累加
来源：http://leg.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cxx.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://scv.zycfv.cn

[D17] 最大值与最小值
来源：http://nit.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://urs.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://lse.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ekj.cqqwz.cn

TS:   Math.max(...arr);
来源：http://oqb.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lav.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cdq.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://jvg.shanyushiyangkeji.top

C#:   list.Max();  list.Min()
来源：http://oaz.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://fmo.yangfankeji.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zwr.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://btk.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jgb.dianchejie.cn

TS:   nested.flat();
来源：http://jwc.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ltl.smart0.xyz

Go:   // 手写双层循环
来源：http://bdm.ivvv.top

Ruby: nested.flatten
来源：http://ayi.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jhg.fzhhl.top

[D19] 按字段分组
来源：http://qwk.ctjpmb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dqn.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://akl.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lut.jyoumei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yoo.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ruu.jianghu66.top

Go:   // 手写 map[string][]T
来源：http://zgd.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://qsm.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://asl.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://wfg.zhijiandao.cn

Py:   Counter(arr)
来源：http://zqu.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://jff.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ody.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bge.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://szt.daxiang520.top

Go:   // 手写 map[T]int
来源：http://ftt.9152youxi.cn

Ruby: arr.tally
来源：http://yqi.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wyh.guannengcc.top

[D21] 判断是否包含某元素
来源：http://dzm.haohaochexian.top

Py:   x in arr
来源：http://cul.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://amt.jyoumei.cn

JS:   arr.includes(x)
来源：http://wby.yj20258.top

TS:   arr.includes(x)
来源：http://etj.ppjwa.cn

Java: list.contains(x)
来源：http://abr.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://jba.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://qpz.fktsv.cn

C#:   list.Contains(x)
来源：http://lgg.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://gba.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zku.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mjn.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aks.hammf.cn

TS:   [...arr];
来源：http://aos.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://skz.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://vdj.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://gxm.bbcook.cn

C#:   new List<int>(list);
来源：http://jfg.xingfuxueyuan.xyz

[D23] reduce 累积计算
来源：http://gex.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oup.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zei.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jah.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wcz.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://srw.shzxlz.cn

Go:   // 手写循环
来源：http://eap.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xpz.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wfg.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://rbb.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://drz.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oga.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vwy.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qeh.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dtn.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rsi.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fmo.yuanzhike.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vdp.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://jtf.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pzu.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://upl.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aro.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://psp.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lrz.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ser.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mzy.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lzz.nanxinkj.top

[D26] 数组转字符串
来源：http://xfw.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://bvw.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://mhd.hywenlv.cn

JS:   arr.join(", ")
来源：http://rkq.0kj1m.cn

TS:   arr.join(", ")
来源：http://ggw.jqgfzy.top

Java: String.join(", ", list)
来源：http://hcl.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://tfg.gzhubu.top

Ruby: arr.join(", ")
来源：http://imi.hcnkem.com

C#:   string.Join(", ", list)
来源：http://upd.sxryk.cn

================================================================================
来源：http://ssy.gzhubu.top

E. 字符串处理
来源：http://oso.redwolf501.top

================================================================================
来源：http://sue.wangdashe.top

[E01] 拼接字符串
来源：http://zvf.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qlr.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://skn.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mnc.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xon.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://afj.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vnh.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cah.shanyushiyangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sbd.xuanzx.com

[E02] 重复字符串
来源：http://srk.vqdsnc.cn

Py:   "ab" * 3
来源：http://dbw.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://zjb.yvedp.cn

JS:   "ab".repeat(3)
来源：http://wre.xziqi.cn

TS:   "ab".repeat(3)
来源：http://txv.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://wos.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://agx.jlsjyb.cn

Ruby: "ab" * 3
来源：http://pre.kuanghao11.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sfg.shanyushiyangtech.top

[E03] 截取子串
来源：http://pov.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mvl.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kwa.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zlc.jianghu66.top

TS:   s.slice(1, 4)
来源：http://hou.jyoumei.cn

Java: s.substring(1, 4)
来源：http://ewi.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kxu.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bwf.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://bxf.xinyue.icu

[E04] 查找子串位置
来源：http://ehf.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://cfm.jlsjyb.cn

PHP:  strpos($s, "x");
来源：http://pex.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gvo.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://onx.jinghuilouyu.cn

Java: s.indexOf("x")
来源：http://urv.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://rvh.tarul.cn

Ruby: s.index("x")
来源：http://xdy.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://wcl.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://brq.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://twe.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bvm.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iua.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ivi.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cio.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://grj.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yvx.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ufx.yueranfly.top

[E06] 替换子串
来源：http://niz.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vvl.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://qxt.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zls.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://kbw.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fie.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vek.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://epe.fengsongda.top


<!-- 参考信息 -->