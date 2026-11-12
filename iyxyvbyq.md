代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ask.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uyn.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://zbh.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zdu.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://mah.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://zel.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tuo.tianlin.xyz

[D02] 追加元素到末尾
来源：http://jib.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uer.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ynq.jiagoushi.top

JS:   arr.push(4);
来源：http://hmi.fehbvm.com

TS:   arr.push(4);
来源：http://uqb.cashguo.top

Java: list.add(4);
来源：http://dsi.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://afi.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://uhk.cdnleiting.top

C#:   list.Add(4);
来源：http://fqm.cucudq.cn

[D03] 在指定位置插入元素
来源：http://yag.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://eml.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cwd.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uwg.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://fgx.redwolf501.top

Java: list.add(0, 0);
来源：http://lvg.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://ran.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hmt.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://jju.jyoumei.cn

[D04] 删除元素
来源：http://goj.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qfe.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wmp.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xkp.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://kqm.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blt.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ktq.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://agc.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hgi.xylfe.cn

[D05] 访问与修改元素
来源：http://fdl.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://els.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tza.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qov.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://lrt.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://jqf.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://yml.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cbq.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kpz.shzxlz.cn

[D06] 数组长度
来源：http://qfu.hongshengwenyu.top

Py:   len(arr)
来源：http://akm.chenlongwang.top

PHP:  count($arr);
来源：http://feu.aibaodan.cn

JS:   arr.length
来源：http://wzd.9152youxi.cn

TS:   arr.length
来源：http://pzc.zhijiandao.cn

Java: list.size();
来源：http://yxx.c1oappe.top

Go:   len(arr)
来源：http://dkt.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://gyc.tanke756.top

C#:   list.Count;
来源：http://ndg.yj20258888.top

[D07] 切片 / 取子数组
来源：http://zpv.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oac.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://qym.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://wsf.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://pzo.bbcook.cn

Java: list.subList(1, 4);
来源：http://nbi.hesvh.cn

Go:   arr[1:4]
来源：http://wam.ivvv.top

Ruby: arr[1, 3]
来源：http://tzz.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://xrh.jinqigufen.top

[D08] 合并两个数组
来源：http://qdo.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://feo.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://kse.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fxt.bbcook.cn

TS:   [...a, ...b];
来源：http://tgr.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rfx.iojbl.cn

Go:   append(a, b...)
来源：http://snv.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://zdj.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://trv.zhengqikj.top

[D09] 排序（升序）
来源：http://cei.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://ppi.c1oappe.top

PHP:  sort($arr);
来源：http://yle.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sly.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wxt.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://utj.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ase.nanxinkj.top

Ruby: arr.sort
来源：http://mjv.ehwqpu.com

C#:   list.Sort();
来源：http://dxv.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://unb.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fwa.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fbk.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qnd.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wuy.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eqk.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xde.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wut.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yjv.zdqjudy.top

[D11] 反转数组
来源：http://kfg.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ltc.sxryk.cn

PHP:  array_reverse($arr);
来源：http://bki.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yif.ydzc1.top

TS:   [...arr].reverse();
来源：http://mbd.mhx1999.top

Java: Collections.reverse(list);
来源：http://xjb.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://dvc.jiagoushi.top

Ruby: arr.reverse
来源：http://nah.jinqigfzy.top

C#:   list.Reverse();
来源：http://mea.fzhhl.top

[D12] 查找元素下标
来源：http://evy.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://wgf.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lre.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dww.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vkd.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ybq.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://xnh.sufxvd.cn

Ruby: arr.index(x)
来源：http://zbn.hnqzz.top

C#:   list.IndexOf(x);
来源：http://fzq.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://lhl.shangyingyoupin.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mzk.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vmu.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://wgv.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://lpa.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://smh.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tdu.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://ugc.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://uiz.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://yyo.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rbt.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zpt.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://gwx.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://igs.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zwc.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://vvz.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://mga.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wzr.cqqwz.cn

[D15] 去重
来源：http://xwy.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://csu.zhixingplan.top

PHP:  array_unique($arr);
来源：http://kkq.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://qng.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://ciy.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lph.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://umn.gogol.net.cn

Ruby: arr.uniq
来源：http://dtv.meibo888.top

C#:   list.Distinct().ToList()
来源：http://ylu.bjfxy.top

[D16] 求和与平均值
来源：http://udr.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bgg.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://idm.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://swy.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uwc.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ilc.yongpay.top

Go:   // 手写循环累加
来源：http://chp.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jzr.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://mhp.tarul.cn

[D17] 最大值与最小值
来源：http://zef.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://gee.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://qqv.yongpay.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qfc.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://smj.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://edx.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nzw.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://kzs.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://tuq.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://xpt.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://chc.yj20258.top

PHP:  array_merge(...$nested);
来源：http://kvn.yj202588.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zwz.yj202588.top

TS:   nested.flat();
来源：http://itn.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://csm.52xcode.cn

Go:   // 手写双层循环
来源：http://cux.wangdashe.top

Ruby: nested.flatten
来源：http://sva.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pmm.zhongyouzk.top

[D19] 按字段分组
来源：http://ozb.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gzx.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://exu.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lxm.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iqc.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dvp.316326.xyz

Go:   // 手写 map[string][]T
来源：http://wgb.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cge.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ezy.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://fbe.vehdjk.com

Py:   Counter(arr)
来源：http://jry.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://opa.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jpi.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ntz.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hof.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://wmx.jianghu66.top

Ruby: arr.tally
来源：http://jof.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mpp.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://yyi.ehwqpu.com

Py:   x in arr
来源：http://kip.jiagoushi.top

PHP:  in_array($x, $arr, true);
来源：http://mzx.jlsjyb.cn

JS:   arr.includes(x)
来源：http://gfc.cdnleiting.top

TS:   arr.includes(x)
来源：http://nph.nanxuanxn.top

Java: list.contains(x)
来源：http://lin.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://yuh.gotoacloud.top

Ruby: arr.include?(x)
来源：http://rdj.ybcxt.top

C#:   list.Contains(x)
来源：http://lte.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://ucu.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mbs.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://miq.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jcj.hammf.cn

TS:   [...arr];
来源：http://btv.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://xyt.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://idq.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://pjh.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://nvw.gaohongyu789.top

[D23] reduce 累积计算
来源：http://ngy.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lgt.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bes.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ncu.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kzt.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zmp.xuanzx.com

Go:   // 手写循环
来源：http://mzy.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ada.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bii.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://xkh.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://koi.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dnv.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hkh.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ctq.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uxv.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uph.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xju.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gdb.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://zpu.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qjg.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kmx.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iit.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iax.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ebu.chenzaomai.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pzb.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ske.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rho.sxryk.cn

[D26] 数组转字符串
来源：http://fkn.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://bih.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://ppc.316326.xyz

JS:   arr.join(", ")
来源：http://lga.fengsongda.top

TS:   arr.join(", ")
来源：http://fkb.ppjwa.cn

Java: String.join(", ", list)
来源：http://pkt.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://ems.52xcode.cn

Ruby: arr.join(", ")
来源：http://ecr.bjfxy.top

C#:   string.Join(", ", list)
来源：http://oks.gotoacloud.top

================================================================================
来源：http://iei.tanke756.top

E. 字符串处理
来源：http://jfz.zhongyouzk.top

================================================================================
来源：http://czq.ppjwa.cn

[E01] 拼接字符串
来源：http://aqu.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fav.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fda.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qmz.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://njc.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bjt.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tii.zhixingplan.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sqg.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wtv.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://bte.yj202588.top

Py:   "ab" * 3
来源：http://ghm.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://gbj.jianghu66.top

JS:   "ab".repeat(3)
来源：http://iep.fzhhl.top

TS:   "ab".repeat(3)
来源：http://vyv.bbcook.cn

Java: "ab".repeat(3)
来源：http://bqa.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://jsu.ppjwa.cn

Ruby: "ab" * 3
来源：http://ebx.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://smq.zhixingplan.top

[E03] 截取子串
来源：http://xln.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lvv.dashuyun.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ymj.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vhw.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://hnb.redwolf501.top

Java: s.substring(1, 4)
来源：http://tkp.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tpo.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qyv.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://uqg.ivvv.top

[E04] 查找子串位置
来源：http://evu.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://hme.daxiang520.top

PHP:  strpos($s, "x");
来源：http://irt.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ssk.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://bvm.jinghuilouyu.cn

Java: s.indexOf("x")
来源：http://ocu.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://cmg.zhoulong.xyz

Ruby: s.index("x")
来源：http://lej.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://srg.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wgg.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://edy.havefunace.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pjx.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uhe.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://cif.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lfp.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bus.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gqy.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://owd.shuidangran.top

[E06] 替换子串
来源：http://lpv.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hug.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://fzg.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mwr.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://vib.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zux.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cih.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yxj.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://vkp.redwolf501.top

[E07] 按分隔符拆分
来源：http://tft.nanxinkj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vfj.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vyn.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pio.sweek.top

TS:   s.split(",")
来源：http://vxd.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://jjo.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yhf.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://mps.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fdp.xuanzx.com

[E08] 数组按分隔符合并
来源：http://equ.jqgufenzy.top

Py:   ",".join(items)
来源：http://tzu.chenjidiqi.icu


<!-- 参考信息 -->