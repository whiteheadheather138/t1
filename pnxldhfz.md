代发 wailian999

PHP:  // 无重载
来源：http://cfh.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qzr.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://mbo.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://kko.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://lyy.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://alc.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zmj.nwbrower.top

================================================================================
来源：http://csr.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://ubj.yonumen.top

================================================================================
来源：http://czh.wangshuangyany.cn

[D01] 创建数组 / 列表
来源：http://fgi.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uco.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yps.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cab.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bnn.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tul.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://zbs.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://iin.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fbw.yvedp.cn

[D02] 追加元素到末尾
来源：http://paf.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kyu.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yzu.jyoumei.cn

JS:   arr.push(4);
来源：http://ygn.hnxiangtu.top

TS:   arr.push(4);
来源：http://irh.xylfe.cn

Java: list.add(4);
来源：http://kum.jianghu66.top

Go:   arr = append(arr, 4)
来源：http://cfh.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://hgs.jianghu66.top

C#:   list.Add(4);
来源：http://vaz.xinyue.icu

[D03] 在指定位置插入元素
来源：http://cpe.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://djp.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uyb.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yei.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://ltt.jiagoushi.top

Java: list.add(0, 0);
来源：http://gca.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://mki.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://axy.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://ruj.daxiang520.top

[D04] 删除元素
来源：http://rcn.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ybm.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ajs.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jxg.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://uyi.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lmn.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yms.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cfo.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xvp.yueranfly.top

[D05] 访问与修改元素
来源：http://rha.yj202588.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iij.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xvl.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kuu.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://rgw.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://dlr.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://fee.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uzj.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://avb.ctjpmb.com

[D06] 数组长度
来源：http://bnm.pycfn.com

Py:   len(arr)
来源：http://jmz.quarkkingdee.top

PHP:  count($arr);
来源：http://uiq.yj20258.top

JS:   arr.length
来源：http://wtn.jinghuilouyu.cn

TS:   arr.length
来源：http://jbv.uphjek.com

Java: list.size();
来源：http://ykp.gotoacloud.top

Go:   len(arr)
来源：http://uyo.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://zee.fanxiaobao.xyz

C#:   list.Count;
来源：http://xpo.redwolf501.top

[D07] 切片 / 取子数组
来源：http://bfj.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ojl.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://wtl.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://tyq.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://bnx.0kj1m.cn

Java: list.subList(1, 4);
来源：http://dan.hysaishi.cn

Go:   arr[1:4]
来源：http://rgr.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://sce.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://nxs.fengsongda.top

[D08] 合并两个数组
来源：http://bvx.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://sod.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://cng.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://nje.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://tye.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xft.hywenlv.cn

Go:   append(a, b...)
来源：http://yhm.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://prr.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://gqw.quarkkingdee.top

[D09] 排序（升序）
来源：http://qak.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://wqz.yuxming.cn

PHP:  sort($arr);
来源：http://ios.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sdh.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vur.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pmk.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rwl.dashuyun.cn

Ruby: arr.sort
来源：http://bmy.chenjidiqi.icu

C#:   list.Sort();
来源：http://rsr.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hfx.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lit.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ytf.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ggm.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bvc.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ycd.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rwj.ywan-chungtsiang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uig.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xtg.hongshengwenyu.top

[D11] 反转数组
来源：http://loj.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dqj.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://bjx.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vai.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://gtl.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://uco.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://bbv.gzhubu.top

Ruby: arr.reverse
来源：http://ajw.ydzc1.top

C#:   list.Reverse();
来源：http://ceu.aibaodan.cn

[D12] 查找元素下标
来源：http://ikd.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://fdb.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nwu.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jda.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aoe.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mof.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://jow.yuxming.cn

Ruby: arr.index(x)
来源：http://ghq.yj20258.top

C#:   list.IndexOf(x);
来源：http://ldv.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://xug.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cfd.shanyushiyangtech.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://obg.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://cvh.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://szn.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rdn.jqgfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jxg.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://fcs.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://faa.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://htk.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qfj.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jrs.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://tcv.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://bnc.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mfo.jyoumei.cn

Go:   // 手写循环
来源：http://oor.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://wzi.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zvx.xuetiantiany.cn

[D15] 去重
来源：http://lbm.hnxiangtu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ssr.zhengqikj.top

PHP:  array_unique($arr);
来源：http://vna.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://vue.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://avw.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tqm.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jqp.sxryk.cn

Ruby: arr.uniq
来源：http://mns.zhaomingkeji.xyz

C#:   list.Distinct().ToList()
来源：http://ydf.jianghu66.top

[D16] 求和与平均值
来源：http://ejt.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qzo.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cmf.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pfw.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ndh.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fzk.bbcook.cn

Go:   // 手写循环累加
来源：http://qdy.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gtb.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://ace.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://dyw.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://xcp.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://rjk.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ztz.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://rsc.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://npz.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zuw.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://qvh.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://pfb.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://xqp.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pqw.pycfn.com

PHP:  array_merge(...$nested);
来源：http://pyd.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xlw.sysykeji.top

TS:   nested.flat();
来源：http://vay.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ofs.c1oappe.top

Go:   // 手写双层循环
来源：http://oim.dashuyun.cn

Ruby: nested.flatten
来源：http://wig.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zxj.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://ynm.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zrc.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eem.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jgi.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iou.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zju.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://urw.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bsw.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fmr.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://weu.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://emp.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://oup.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://may.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pjt.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nrg.bbcook.cn

Go:   // 手写 map[T]int
来源：http://ulx.cashguo.top

Ruby: arr.tally
来源：http://moc.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tcx.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://utg.zdbjq.cn

Py:   x in arr
来源：http://djx.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://xhr.yfazqb.com

JS:   arr.includes(x)
来源：http://ybo.epnwcf.com

TS:   arr.includes(x)
来源：http://oxt.nwbrower.top

Java: list.contains(x)
来源：http://teu.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://gri.fehbvm.com

Ruby: arr.include?(x)
来源：http://ban.meibo888.top

C#:   list.Contains(x)
来源：http://pee.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://oue.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kcy.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lue.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ejj.shanyushiyangkeji.top

TS:   [...arr];
来源：http://ilz.xylfe.cn

Java: new ArrayList<>(list);
来源：http://yiq.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://fzs.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://igc.jinqigufen.top

C#:   new List<int>(list);
来源：http://cus.snrcjt.cn

[D23] reduce 累积计算
来源：http://opj.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://emb.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ngh.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eje.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xbc.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cfj.bjfxy.top

Go:   // 手写循环
来源：http://cxx.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pea.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hmx.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://qjw.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hlc.bbcook.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gcu.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tyv.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tjy.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://abz.c1oappe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wpi.yj202588.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uxr.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://obn.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://bum.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hac.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qyw.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fya.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bwv.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://esb.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jlj.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dfy.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://edt.bbcook.cn

[D26] 数组转字符串
来源：http://yrn.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://elq.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://ifb.ivvv.top

JS:   arr.join(", ")
来源：http://ubw.hesvh.cn

TS:   arr.join(", ")
来源：http://rml.kuanghao11.cn

Java: String.join(", ", list)
来源：http://frg.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://vvq.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://ica.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://yko.yangfankeji.com

================================================================================
来源：http://jmk.daria6918.cn

E. 字符串处理
来源：http://glb.yonumen.top

================================================================================
来源：http://fgw.9152youxi.cn

[E01] 拼接字符串
来源：http://thz.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ylq.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://amo.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nav.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qqh.cdnleiting.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gxv.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xbc.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rgm.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jdt.dianchejie.cn

[E02] 重复字符串
来源：http://neu.gotoacloud.top

Py:   "ab" * 3
来源：http://wpa.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://zxg.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://qid.uphjek.com

TS:   "ab".repeat(3)
来源：http://wzb.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://kph.yueranfly.top

Go:   strings.Repeat("ab", 3)
来源：http://uwq.jinqigfzy.top

Ruby: "ab" * 3
来源：http://ztt.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tub.hesvh.cn

[E03] 截取子串
来源：http://jue.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dgh.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bij.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vxp.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://hgr.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://eha.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://clu.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://sxu.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://iwr.xziqi.cn

[E04] 查找子串位置
来源：http://ree.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://nwm.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://wqs.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fwj.vehdjk.com

TS:   s.indexOf("x")
来源：http://edo.havefunace.top

Java: s.indexOf("x")
来源：http://phb.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://mpj.havefunace.top

Ruby: s.index("x")
来源：http://oib.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://egg.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hov.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hub.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xqh.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dzv.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://muy.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vjd.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ruk.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://osq.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ksp.316326.xyz

[E06] 替换子串
来源：http://ipg.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ivj.smart0.xyz

PHP:  str_replace("a", "b", $s);
来源：http://dpw.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rrt.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://aun.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://onv.hnqzz.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://awe.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://btl.mhx1999.top


<!-- 参考信息 -->