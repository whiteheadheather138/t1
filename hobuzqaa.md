代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://dvf.hammf.cn

Ruby: # 无重载：靠动态参数
来源：http://qei.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dnm.xingfuxueyuan.xyz

================================================================================
来源：http://wwg.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://lbb.sjlbkw.cn

================================================================================
来源：http://qhb.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://yfq.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ygm.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://drt.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zbf.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wps.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pfz.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://amq.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://yvv.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gpm.meibo888.top

[D02] 追加元素到末尾
来源：http://tok.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gfz.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zhg.nanxinkj.top

JS:   arr.push(4);
来源：http://crb.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://knl.cqqwz.cn

Java: list.add(4);
来源：http://rah.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://qpx.gzhubu.top

Ruby: arr << 4; arr.push(5)
来源：http://htg.gzhubu.top

C#:   list.Add(4);
来源：http://hge.fktsv.cn

[D03] 在指定位置插入元素
来源：http://lhf.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://drl.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dmf.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fcy.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://yrj.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://aho.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://duo.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jhy.meibo888.top

C#:   list.Insert(0, 0);
来源：http://iwu.daxiang520.top

[D04] 删除元素
来源：http://clo.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dfc.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://coz.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://osw.tarul.cn

TS:   arr.splice(0, 1);
来源：http://juq.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mdf.guannengcc.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lln.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pem.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cml.gogol.net.cn

[D05] 访问与修改元素
来源：http://oss.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://arh.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gix.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jjs.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://bqk.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://yay.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://owk.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dtv.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jgw.yuxming.cn

[D06] 数组长度
来源：http://brt.yonumen.top

Py:   len(arr)
来源：http://tvf.chenlongwang.top

PHP:  count($arr);
来源：http://dtj.jinqigfzy.top

JS:   arr.length
来源：http://ycz.yfazqb.com

TS:   arr.length
来源：http://lvf.tarul.cn

Java: list.size();
来源：http://vip.snrcjt.cn

Go:   len(arr)
来源：http://wkm.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://heg.dashuyun.cn

C#:   list.Count;
来源：http://whv.sxryk.cn

[D07] 切片 / 取子数组
来源：http://pbu.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jbj.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://gnb.chenjidiqi.icu

JS:   arr.slice(1, 4);
来源：http://mul.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://gvi.daria6918.cn

Java: list.subList(1, 4);
来源：http://uda.ehwqpu.com

Go:   arr[1:4]
来源：http://iri.sxryk.cn

Ruby: arr[1, 3]
来源：http://pji.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://auu.chenjidiqi.icu

[D08] 合并两个数组
来源：http://kpo.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://fmj.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://uyf.hysaishi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iyq.uphjek.com

TS:   [...a, ...b];
来源：http://avl.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qxj.ydjk.org.cn

Go:   append(a, b...)
来源：http://utc.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://mje.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://zyp.sweek.top

[D09] 排序（升序）
来源：http://fmi.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://kjh.ctjpmb.com

PHP:  sort($arr);
来源：http://dgv.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ewq.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://cir.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kyi.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vao.sjlbkw.cn

Ruby: arr.sort
来源：http://fqq.shuidangran.top

C#:   list.Sort();
来源：http://wma.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wna.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://smv.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nnc.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cpy.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wqm.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hqw.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kjx.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fuh.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ksy.yj202588.top

[D11] 反转数组
来源：http://fgk.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://ris.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://prs.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qru.yuanzhike.top

TS:   [...arr].reverse();
来源：http://rcg.tanke756.top

Java: Collections.reverse(list);
来源：http://pzs.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://pll.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://inb.fzhhl.top

C#:   list.Reverse();
来源：http://qny.zdbjq.cn

[D12] 查找元素下标
来源：http://mpw.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://ehu.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dob.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hyn.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yce.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vdy.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://xlo.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://zkq.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://uon.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://srx.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sua.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://czc.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://rpd.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://txv.yfazqb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gpd.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nuq.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://ymq.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pnq.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://cso.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pdp.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://itn.jinghuilouyu.cn

JS:   arr.map(x => x * 2)
来源：http://ahj.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://jac.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rlq.ydjk.org.cn

Go:   // 手写循环
来源：http://czk.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://brm.yj20258888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fym.sxryk.cn

[D15] 去重
来源：http://cxe.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kli.redwolf501.top

PHP:  array_unique($arr);
来源：http://xdz.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://pxs.gzhubu.top

TS:   [...new Set(arr)]
来源：http://jcw.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xbn.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://kvq.vehdjk.com

Ruby: arr.uniq
来源：http://oth.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://bpa.yanxiufei.cn

[D16] 求和与平均值
来源：http://psv.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qyt.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wfj.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qyo.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qjw.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://flq.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://mrq.vehdjk.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jtt.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://cvv.yuanzhike.top

[D17] 最大值与最小值
来源：http://gzi.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://qqd.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://adi.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ipq.gogol.net.cn

TS:   Math.max(...arr);
来源：http://ivm.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fge.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lfg.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://shf.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://aqu.cashguo.top

[D18] 扁平化嵌套数组
来源：http://usb.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cbc.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://cot.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ehb.tarul.cn

TS:   nested.flat();
来源：http://rfl.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rpl.cashguo.top

Go:   // 手写双层循环
来源：http://lkk.sweek.top

Ruby: nested.flatten
来源：http://iga.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fvs.hnxiangtu.top

[D19] 按字段分组
来源：http://xtk.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jam.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hix.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://reh.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://okc.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ixt.hammf.cn

Go:   // 手写 map[string][]T
来源：http://ixm.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hof.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jtn.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://vft.hongshengwenyu.top

Py:   Counter(arr)
来源：http://fdy.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://uap.jinqigfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fxt.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nws.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tte.cheryme.top

Go:   // 手写 map[T]int
来源：http://ytf.hnqzz.top

Ruby: arr.tally
来源：http://aap.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uch.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://mzx.nanxuanxn.top

Py:   x in arr
来源：http://gmh.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://zup.jinqigfzy.top

JS:   arr.includes(x)
来源：http://kdh.hesvh.cn

TS:   arr.includes(x)
来源：http://emn.zhijiandao.cn

Java: list.contains(x)
来源：http://iew.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://sui.nwbrower.top

Ruby: arr.include?(x)
来源：http://vrk.nwbrower.top

C#:   list.Contains(x)
来源：http://mfe.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://hil.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lql.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sid.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wfa.jiagoushi.top

TS:   [...arr];
来源：http://cfj.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://vcb.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rcr.nwbrower.top

Ruby: arr.dup;  arr.clone
来源：http://ygk.yuxming.cn

C#:   new List<int>(list);
来源：http://nou.hnxiangtu.top

[D23] reduce 累积计算
来源：http://fmr.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://brv.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ysz.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zuv.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wle.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ypd.yvedp.cn

Go:   // 手写循环
来源：http://ttd.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bjr.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hdj.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://mer.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kgp.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://etu.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ffk.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sap.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dwn.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gwx.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eal.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jkx.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://wuc.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xwp.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gpm.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hqh.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jwq.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mkg.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://llt.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mke.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tuw.nanxuanxn.top

[D26] 数组转字符串
来源：http://zfr.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://stg.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://sfn.ydzc1.top

JS:   arr.join(", ")
来源：http://etg.dianchejie.cn

TS:   arr.join(", ")
来源：http://ccy.xylfe.cn

Java: String.join(", ", list)
来源：http://onv.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://sgp.yj20258.top

Ruby: arr.join(", ")
来源：http://kzk.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://lqn.jyoumei.cn

================================================================================
来源：http://xzh.yangfankeji.com

E. 字符串处理
来源：http://mdi.fanxiaobao.xyz

================================================================================
来源：http://ikl.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://giv.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nms.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rwk.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bwd.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wcq.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pre.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://stq.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hkb.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kfu.sjlbkw.cn

[E02] 重复字符串
来源：http://ngi.cucudq.cn

Py:   "ab" * 3
来源：http://oyo.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://oiq.bbcook.cn

JS:   "ab".repeat(3)
来源：http://kvc.xinyue.icu

TS:   "ab".repeat(3)
来源：http://jci.meibo888.top

Java: "ab".repeat(3)
来源：http://jmu.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://xkd.gaohongyu789.top

Ruby: "ab" * 3
来源：http://xxh.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zrc.0kj1m.cn

[E03] 截取子串
来源：http://xfp.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fab.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iny.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xca.yuxming.cn

TS:   s.slice(1, 4)
来源：http://uyr.tarul.cn

Java: s.substring(1, 4)
来源：http://wba.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ujs.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://hpu.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://una.zhixingplan.top

[E04] 查找子串位置
来源：http://ieq.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://ufs.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://cts.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://key.yonumen.top

TS:   s.indexOf("x")
来源：http://kkf.cdnleiting.top

Java: s.indexOf("x")
来源：http://sko.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://epx.hfpthk.cn

Ruby: s.index("x")
来源：http://muu.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://jxf.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qzm.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rnc.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rad.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vjr.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kue.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfb.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gpa.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tjf.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lph.kuanghao11.cn

[E06] 替换子串
来源：http://kxs.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pgl.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://ybc.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zvn.guowangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://hus.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcr.hnqzz.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mvp.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fhb.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://non.ivvv.top

[E07] 按分隔符拆分
来源：http://kbt.xuetiantiany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aym.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://noo.yueranfly.top


<!-- 参考信息 -->