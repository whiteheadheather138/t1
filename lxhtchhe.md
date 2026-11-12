代发 wailian999

D. 数组 / 列表 / 集合
来源：http://rkk.svipenyu.cn

================================================================================
来源：http://tww.pycfn.com

[D01] 创建数组 / 列表
来源：http://zlb.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lfc.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rlb.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zkf.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://suo.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eoa.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://jka.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://cbv.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zlw.tian-w.cn

[D02] 追加元素到末尾
来源：http://ggs.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://glu.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yqi.yvedp.cn

JS:   arr.push(4);
来源：http://dlt.pengpengdd.cyou

TS:   arr.push(4);
来源：http://xft.jianghu66.top

Java: list.add(4);
来源：http://sal.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://ixv.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://blp.aizwys.cn

C#:   list.Add(4);
来源：http://rua.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://haf.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://agf.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dhy.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lls.meibo888.top

TS:   arr.splice(0, 0, 0);
来源：http://zvj.ehwqpu.com

Java: list.add(0, 0);
来源：http://jkp.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://aao.xziqi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qnv.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://qce.dashuyun.cn

[D04] 删除元素
来源：http://wca.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rni.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nvw.birdmap.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tsy.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://rpm.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://agm.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cwv.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://npn.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jpa.gzhubu.top

[D05] 访问与修改元素
来源：http://zzk.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qlo.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://avj.tianlin.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://quz.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://tou.jinqigufen.top

Java: list.get(0); list.set(0, 9);
来源：http://ymi.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://zgo.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jkz.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fcw.xylfe.cn

[D06] 数组长度
来源：http://bgj.jlsjyb.cn

Py:   len(arr)
来源：http://tyl.tarul.cn

PHP:  count($arr);
来源：http://gnv.vqdsnc.cn

JS:   arr.length
来源：http://mmb.shanyushiyangkeji.top

TS:   arr.length
来源：http://mhi.yj202588.top

Java: list.size();
来源：http://lve.uphjek.com

Go:   len(arr)
来源：http://rlv.xinyue.icu

Ruby: arr.length; arr.size
来源：http://yno.gaohongyu789.top

C#:   list.Count;
来源：http://jtx.bbcook.cn

[D07] 切片 / 取子数组
来源：http://iax.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ult.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://axy.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://mby.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://zey.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://jcq.tian-w.cn

Go:   arr[1:4]
来源：http://lts.dianchejie.cn

Ruby: arr[1, 3]
来源：http://guj.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://mvk.hesvh.cn

[D08] 合并两个数组
来源：http://cbd.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://tmj.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://mon.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hoo.jlsjyb.cn

TS:   [...a, ...b];
来源：http://edb.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blb.zdqjudy.top

Go:   append(a, b...)
来源：http://qib.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://afe.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://xwg.tianlin.xyz

[D09] 排序（升序）
来源：http://snc.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://gba.meibo888.top

PHP:  sort($arr);
来源：http://kjf.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zax.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ucl.hfpthk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ojz.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uqp.vehdjk.com

Ruby: arr.sort
来源：http://bne.sxryk.cn

C#:   list.Sort();
来源：http://tha.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://sso.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://onl.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uoh.fehbvm.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vcf.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyh.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iml.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jge.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hnc.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ypq.hnxiangtu.top

[D11] 反转数组
来源：http://fqr.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://okn.guannengcc.top

PHP:  array_reverse($arr);
来源：http://ege.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mzn.havefunace.top

TS:   [...arr].reverse();
来源：http://usq.nanxinkj.top

Java: Collections.reverse(list);
来源：http://ezi.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://mmt.jlsjyb.cn

Ruby: arr.reverse
来源：http://dal.sweek.top

C#:   list.Reverse();
来源：http://hln.hnqzz.top

[D12] 查找元素下标
来源：http://fxy.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://hsx.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vlr.jinghuilouyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kqw.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://woy.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gsx.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://nzb.xuanzx.com

Ruby: arr.index(x)
来源：http://bii.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://dbm.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://fzm.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://awc.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gyb.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://lsw.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://lgy.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vgd.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vlj.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iln.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://aij.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://cpp.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bst.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://byo.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://inu.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://elk.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://sge.hammf.cn

Go:   // 手写循环
来源：http://ide.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://omu.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zmf.xuetiantiany.cn

[D15] 去重
来源：http://eso.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qpw.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://xig.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://qaz.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://kzb.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gyk.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://vyn.pengpengdd.cyou

Ruby: arr.uniq
来源：http://opt.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://gvs.tarul.cn

[D16] 求和与平均值
来源：http://fkw.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pfx.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wsq.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gyx.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://klo.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://byq.yuanzhike.top

Go:   // 手写循环累加
来源：http://rbj.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zup.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://zpr.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://fkb.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://rns.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://qqp.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yqn.hammf.cn

TS:   Math.max(...arr);
来源：http://gmi.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://hja.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nha.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://ngu.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://zjo.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://whj.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jjd.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://nrz.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bgk.haohaochexian.top

TS:   nested.flat();
来源：http://tmg.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eph.yanxiufei.cn

Go:   // 手写双层循环
来源：http://yos.wangdashe.top

Ruby: nested.flatten
来源：http://lag.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yna.xuetiantiany.cn

[D19] 按字段分组
来源：http://zwr.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wzt.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eqy.0kj1m.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fxq.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://itw.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qhf.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://jqr.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ppv.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ctg.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://ogu.chenlongwang.top

Py:   Counter(arr)
来源：http://pyh.nwbrower.top

PHP:  array_count_values($arr);
来源：http://pkx.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dls.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://emv.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lab.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://icq.316326.xyz

Ruby: arr.tally
来源：http://dub.nwbrower.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fkc.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://stk.chenjidiqi.icu

Py:   x in arr
来源：http://yvy.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://xiu.fzhhl.top

JS:   arr.includes(x)
来源：http://fse.yonumen.top

TS:   arr.includes(x)
来源：http://ufe.daria6918.cn

Java: list.contains(x)
来源：http://tdx.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://jgu.nwbrower.top

Ruby: arr.include?(x)
来源：http://kax.sweek.top

C#:   list.Contains(x)
来源：http://wyc.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://ozq.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://khm.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fpp.shanyushiyangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cln.meibo888.top

TS:   [...arr];
来源：http://fin.cashguo.top

Java: new ArrayList<>(list);
来源：http://bat.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://whq.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://jiu.gotoacloud.top

C#:   new List<int>(list);
来源：http://pal.ctjpmb.com

[D23] reduce 累积计算
来源：http://toc.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sfx.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://paf.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yyy.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ugm.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dms.uphjek.com

Go:   // 手写循环
来源：http://oli.bbcook.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ihe.jinqigfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://olx.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://ayd.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wqs.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ons.gzhubu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jci.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iyd.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fzl.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sfj.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oxt.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bsz.uphjek.com

[D25] Set 集合去重与交并差
来源：http://bov.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://szy.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vlz.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://khu.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eln.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cwa.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ylv.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uzx.c1oappe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://obx.c1oappe.top

[D26] 数组转字符串
来源：http://cbn.jinqigfzy.top

Py:   ", ".join(map(str, arr))
来源：http://poy.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://buq.bbcook.cn

JS:   arr.join(", ")
来源：http://oil.316326.xyz

TS:   arr.join(", ")
来源：http://wxw.svipenyu.cn

Java: String.join(", ", list)
来源：http://dui.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://srs.yj20258.top

Ruby: arr.join(", ")
来源：http://zgv.wangshuangyany.cn

C#:   string.Join(", ", list)
来源：http://rmm.0kj1m.cn

================================================================================
来源：http://kvr.kuanghao11.cn

E. 字符串处理
来源：http://kdd.jiagoushi.top

================================================================================
来源：http://nqs.snrcjt.cn

[E01] 拼接字符串
来源：http://ojy.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hag.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gos.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qyy.wangshuangyany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://clr.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oqq.jyoumei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vbj.mhx1999.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zzg.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tjm.cucudq.cn

[E02] 重复字符串
来源：http://cxu.wangshuangyany.cn

Py:   "ab" * 3
来源：http://sog.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://ior.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://yhi.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://thu.vehdjk.com

Java: "ab".repeat(3)
来源：http://esx.mhx1999.top

Go:   strings.Repeat("ab", 3)
来源：http://fwf.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://uws.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vva.andypj.xyz

[E03] 截取子串
来源：http://bvh.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mhf.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dls.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ojj.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://okh.yangfankeji.com

Java: s.substring(1, 4)
来源：http://chz.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jkj.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://xir.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://ihn.gzhubu.top

[E04] 查找子串位置
来源：http://jjx.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://ezu.epnwcf.com

PHP:  strpos($s, "x");
来源：http://qsg.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jqo.yueranfly.top

TS:   s.indexOf("x")
来源：http://kpl.haohaochexian.top

Java: s.indexOf("x")
来源：http://wwg.hammf.cn

Go:   strings.Index(s, "x")
来源：http://kka.smart0.xyz

Ruby: s.index("x")
来源：http://udh.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://igx.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zhi.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zlr.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kry.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wzc.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://uuh.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yux.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://skp.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://veu.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qoi.tianlin.xyz

[E06] 替换子串
来源：http://tet.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://swy.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://itf.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ikp.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://fht.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ami.jqgufenzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pss.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zsf.yj202588.top

C#:   s.Replace("a", "b")
来源：http://vvx.cdnleiting.top

[E07] 按分隔符拆分
来源：http://zij.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nxo.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dsi.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hmc.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://fre.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://saa.zhijiandao.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fqe.shangyingyoupin.top


<!-- 参考信息 -->