代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qpe.yuxming.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qtg.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://drg.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tcl.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://jrr.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://qgw.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tki.sufxvd.cn

[D02] 追加元素到末尾
来源：http://ssr.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cbf.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nte.ehwqpu.com

JS:   arr.push(4);
来源：http://xdm.yuanzhike.top

TS:   arr.push(4);
来源：http://tkv.smart0.xyz

Java: list.add(4);
来源：http://fru.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://fcb.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://eel.ppjwa.cn

C#:   list.Add(4);
来源：http://fuz.tian-w.cn

[D03] 在指定位置插入元素
来源：http://htk.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://yyu.jlsjyb.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pxx.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yqe.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://fto.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://igz.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://ddl.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fcc.jinqigfzy.top

C#:   list.Insert(0, 0);
来源：http://gtn.ivvv.top

[D04] 删除元素
来源：http://rgl.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uzb.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aok.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fga.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://flq.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xdw.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ktd.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vbv.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://isa.jianghu66.top

[D05] 访问与修改元素
来源：http://try.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wfz.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mym.yueranfly.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ixe.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://lvv.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://cqv.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://cgh.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hjo.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://exe.aibaodan.cn

[D06] 数组长度
来源：http://gnk.sufxvd.cn

Py:   len(arr)
来源：http://fiz.hfpthk.cn

PHP:  count($arr);
来源：http://wti.ydjk.org.cn

JS:   arr.length
来源：http://evn.hywenlv.cn

TS:   arr.length
来源：http://ndt.dashuyun.cn

Java: list.size();
来源：http://qph.gotoacloud.top

Go:   len(arr)
来源：http://hgf.xinyue.icu

Ruby: arr.length; arr.size
来源：http://ate.tianlin.xyz

C#:   list.Count;
来源：http://ndb.guannengcc.top

[D07] 切片 / 取子数组
来源：http://itw.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hen.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://jae.0kj1m.cn

JS:   arr.slice(1, 4);
来源：http://mof.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://upb.wangdashe.top

Java: list.subList(1, 4);
来源：http://ecr.vehdjk.com

Go:   arr[1:4]
来源：http://jwu.cdnleiting.top

Ruby: arr[1, 3]
来源：http://qxz.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://kwi.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://xnd.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://hjo.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://nll.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zcq.yonumen.top

TS:   [...a, ...b];
来源：http://gql.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lyb.jinqigufen.top

Go:   append(a, b...)
来源：http://jnt.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://izg.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://dvo.hnqzz.top

[D09] 排序（升序）
来源：http://epe.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://jcy.vehdjk.com

PHP:  sort($arr);
来源：http://ijr.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://krl.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tzs.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dge.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bvk.sysykeji.top

Ruby: arr.sort
来源：http://pme.bjfxy.top

C#:   list.Sort();
来源：http://nkq.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://knx.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jpa.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jyo.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iva.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oqf.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jpc.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lak.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hxp.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gzc.bbcook.cn

[D11] 反转数组
来源：http://qeg.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://rgb.pycfn.com

PHP:  array_reverse($arr);
来源：http://zgs.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lnr.daxiang520.top

TS:   [...arr].reverse();
来源：http://kpi.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://kqi.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://ijg.jlsjyb.cn

Ruby: arr.reverse
来源：http://okt.hcnkem.com

C#:   list.Reverse();
来源：http://yzf.316326.xyz

[D12] 查找元素下标
来源：http://mhc.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://thr.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://efo.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://owx.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oiv.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kxl.yangfankeji.com

Go:   slices.Index(arr, x)
来源：http://alz.yanxiufei.cn

Ruby: arr.index(x)
来源：http://bnz.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://nqq.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://ati.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ntb.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zlp.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://htd.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://wly.yj20258.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gja.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fav.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://gov.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bja.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://hgn.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xgz.jyoumei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nyj.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://gsq.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://tvk.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hgr.fehbvm.com

Go:   // 手写循环
来源：http://glx.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://xth.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nvu.ctjpmb.com

[D15] 去重
来源：http://mob.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ymz.jqgfzy.top

PHP:  array_unique($arr);
来源：http://jeo.shuidangran.top

JS:   [...new Set(arr)]
来源：http://vzr.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://kjp.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yri.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yfp.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://zkv.uphjek.com

C#:   list.Distinct().ToList()
来源：http://rea.xylfe.cn

[D16] 求和与平均值
来源：http://kfj.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dze.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://flx.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iig.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://npw.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qhe.quarkkingdee.top

Go:   // 手写循环累加
来源：http://gga.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nav.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://pcv.bbcook.cn

[D17] 最大值与最小值
来源：http://udh.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://vjt.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://rsm.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mgl.snrcjt.cn

TS:   Math.max(...arr);
来源：http://rkh.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ejv.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://axq.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://koo.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://ccd.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://evz.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://apc.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://aar.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sqx.zhengqikj.top

TS:   nested.flat();
来源：http://bkh.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mlf.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://wiq.yuxming.cn

Ruby: nested.flatten
来源：http://ypx.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iuc.sysykeji.top

[D19] 按字段分组
来源：http://kff.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nvt.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uqe.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fru.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ttm.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zqw.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://dms.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://mca.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://srb.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://bkn.daxiang520.top

Py:   Counter(arr)
来源：http://mmb.yfazqb.com

PHP:  array_count_values($arr);
来源：http://yvy.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uuo.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rcy.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jac.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://bpi.zdqjudy.top

Ruby: arr.tally
来源：http://xds.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xvz.hcnkem.com

[D21] 判断是否包含某元素
来源：http://asg.dashuyun.cn

Py:   x in arr
来源：http://xwj.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://nev.redwolf501.top

JS:   arr.includes(x)
来源：http://jbx.dianchejie.cn

TS:   arr.includes(x)
来源：http://fcb.hongshengwenyu.top

Java: list.contains(x)
来源：http://zfz.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://sns.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://xjs.nanxinkj.top

C#:   list.Contains(x)
来源：http://jsm.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://zhg.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nfd.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zmm.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ogs.dianchejie.cn

TS:   [...arr];
来源：http://xjc.tanke756.top

Java: new ArrayList<>(list);
来源：http://nta.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uge.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://ycd.tarul.cn

C#:   new List<int>(list);
来源：http://azd.havefunace.top

[D23] reduce 累积计算
来源：http://jyf.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gyi.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vjc.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bmg.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mxt.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xat.guannengcc.top

Go:   // 手写循环
来源：http://aic.ywan-chungtsiang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ryz.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hfh.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://tci.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hbw.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lbn.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nqv.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mcx.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rin.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pfq.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gnf.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aap.havefunace.top

[D25] Set 集合去重与交并差
来源：http://jbp.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nnq.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dlt.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://grf.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lnn.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dmc.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://syd.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nrn.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xha.iojbl.cn

[D26] 数组转字符串
来源：http://ssx.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://ezr.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://ven.meibo888.top

JS:   arr.join(", ")
来源：http://tqv.vqdsnc.cn

TS:   arr.join(", ")
来源：http://cum.fengsongda.top

Java: String.join(", ", list)
来源：http://yii.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://wzp.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://ckq.wangdashe.top

C#:   string.Join(", ", list)
来源：http://kwp.chenlongwang.top

================================================================================
来源：http://lpp.hongshengwenyu.top

E. 字符串处理
来源：http://bmb.aibaodan.cn

================================================================================
来源：http://yha.jiagoushi.top

[E01] 拼接字符串
来源：http://wvh.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://flc.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eiy.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hge.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zwh.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uze.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iaw.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lkv.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ize.guowangkeji.top

[E02] 重复字符串
来源：http://ajo.yonumen.top

Py:   "ab" * 3
来源：http://vgb.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://yyj.xylfe.cn

JS:   "ab".repeat(3)
来源：http://iwy.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://brh.316326.xyz

Java: "ab".repeat(3)
来源：http://mwp.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://uox.shuidangran.top

Ruby: "ab" * 3
来源：http://gim.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://etj.ybcxt.top

[E03] 截取子串
来源：http://bmt.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qrh.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sbk.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tnf.yvedp.cn

TS:   s.slice(1, 4)
来源：http://cxf.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://neb.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://khb.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://lyk.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://zuh.shzxlz.cn

[E04] 查找子串位置
来源：http://fpv.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://nxm.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://huu.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ylb.smart0.xyz

TS:   s.indexOf("x")
来源：http://vpz.aibaodan.cn

Java: s.indexOf("x")
来源：http://lbp.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://dcg.iojbl.cn

Ruby: s.index("x")
来源：http://mis.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://wjw.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://dbk.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://csk.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bco.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tvj.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bwa.xingfuxueyuan.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qak.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ika.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ood.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ypx.iojbl.cn

[E06] 替换子串
来源：http://ash.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://izx.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://xbw.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bre.haohaochexian.top

TS:   s.replaceAll("a", "b")
来源：http://huo.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ixd.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nhz.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ijb.yj20258.top

C#:   s.Replace("a", "b")
来源：http://mks.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://erg.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rpg.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jzc.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qcf.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://iww.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://btc.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zzw.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://lhm.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jvn.redwolf501.top

[E08] 数组按分隔符合并
来源：http://syk.vehdjk.com

Py:   ",".join(items)
来源：http://gay.birdmap.top


<!-- 参考信息 -->