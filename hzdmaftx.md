代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://rri.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://vzk.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cga.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://pja.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hft.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ewf.zycfv.cn

JS:   arr.push(4);
来源：http://wsg.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://uki.gaohongyu789.top

Java: list.add(4);
来源：http://odh.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://vyu.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://fbp.daria6918.cn

C#:   list.Add(4);
来源：http://qms.hammf.cn

[D03] 在指定位置插入元素
来源：http://jky.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://elw.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ejb.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tsg.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://myw.bbcook.cn

Java: list.add(0, 0);
来源：http://ord.jiagoushi.top

Go:   arr = append([]int{0}, arr...)
来源：http://nju.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ocs.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://bas.ppjwa.cn

[D04] 删除元素
来源：http://msf.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ceb.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dik.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ebf.yuxming.cn

TS:   arr.splice(0, 1);
来源：http://nmf.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ldm.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ibj.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hdj.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mnm.dianchejie.cn

[D05] 访问与修改元素
来源：http://gyr.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hbw.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vef.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oeq.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://pmd.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://vnw.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://hpf.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gde.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wqh.gaohongyu789.top

[D06] 数组长度
来源：http://tle.ydjk.org.cn

Py:   len(arr)
来源：http://iaw.fengsongda.top

PHP:  count($arr);
来源：http://nhy.aibaodan.cn

JS:   arr.length
来源：http://mxg.pycfn.com

TS:   arr.length
来源：http://utx.ywan-chungtsiang.top

Java: list.size();
来源：http://cba.ybcxt.top

Go:   len(arr)
来源：http://ahd.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://ugn.mhx1999.top

C#:   list.Count;
来源：http://ypu.bjfxy.top

[D07] 切片 / 取子数组
来源：http://agu.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gve.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://opx.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://qwo.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://boy.9152youxi.cn

Java: list.subList(1, 4);
来源：http://upg.jqgufenzy.top

Go:   arr[1:4]
来源：http://hvx.ivvv.top

Ruby: arr[1, 3]
来源：http://hjc.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://vhz.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://cyx.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://vax.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://grk.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://heu.havefunace.top

TS:   [...a, ...b];
来源：http://eun.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pos.yfazqb.com

Go:   append(a, b...)
来源：http://ryw.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://ego.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://ixh.dianchejie.cn

[D09] 排序（升序）
来源：http://scs.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://ues.mhx1999.top

PHP:  sort($arr);
来源：http://xsn.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gvx.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tdr.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ipk.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://slf.smart0.xyz

Ruby: arr.sort
来源：http://smv.redwolf501.top

C#:   list.Sort();
来源：http://btc.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tep.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jol.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uhh.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iml.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://buq.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qeg.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qdi.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yar.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yfy.fanxiaobao.xyz

[D11] 反转数组
来源：http://bza.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://dzy.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://oqr.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://olj.fktsv.cn

TS:   [...arr].reverse();
来源：http://rkt.ctjpmb.com

Java: Collections.reverse(list);
来源：http://rbz.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://llh.wangshuangyany.cn

Ruby: arr.reverse
来源：http://spk.fktsv.cn

C#:   list.Reverse();
来源：http://vux.zdbjq.cn

[D12] 查找元素下标
来源：http://nde.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://ndb.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hvm.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rlb.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wge.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fqc.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://ajw.hnxiangtu.top

Ruby: arr.index(x)
来源：http://ztd.fktsv.cn

C#:   list.IndexOf(x);
来源：http://rrr.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://vvp.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yda.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kts.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://nyy.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://equ.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lcv.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yql.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jek.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://dtg.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://mbj.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bdd.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://txp.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://qko.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://vlm.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xwb.hesvh.cn

Go:   // 手写循环
来源：http://cgt.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dbu.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yfp.ydjk.org.cn

[D15] 去重
来源：http://mhs.aibaodan.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lwp.jinyuanbaomall.cn

PHP:  array_unique($arr);
来源：http://seh.52xcode.cn

JS:   [...new Set(arr)]
来源：http://ves.yuxming.cn

TS:   [...new Set(arr)]
来源：http://mbe.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://djc.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xub.guowangkeji.top

Ruby: arr.uniq
来源：http://kdp.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://nzh.yj20258888.top

[D16] 求和与平均值
来源：http://hgw.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bch.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ono.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://knr.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://roj.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hxv.wangdashe.top

Go:   // 手写循环累加
来源：http://hag.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eox.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://moe.zhixingplan.top

[D17] 最大值与最小值
来源：http://his.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://tkh.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://lwv.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zug.hesvh.cn

TS:   Math.max(...arr);
来源：http://dkl.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ibt.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xkk.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://lbh.cashguo.top

C#:   list.Max();  list.Min()
来源：http://xjg.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://hew.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bnr.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://tvy.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dey.zhengqikj.top

TS:   nested.flat();
来源：http://kus.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nlk.sufxvd.cn

Go:   // 手写双层循环
来源：http://fad.shzxlz.cn

Ruby: nested.flatten
来源：http://orp.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://qui.zhixingplan.top

[D19] 按字段分组
来源：http://aoj.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://htb.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rzq.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tor.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://evw.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jgt.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://chy.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oyt.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sfi.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://lho.gzhubu.top

Py:   Counter(arr)
来源：http://wph.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://uet.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oii.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://isj.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hoe.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://hyz.aibaodan.cn

Ruby: arr.tally
来源：http://lhi.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mco.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://kuc.ywan-chungtsiang.top

Py:   x in arr
来源：http://ulk.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://irk.guowangkeji.top

JS:   arr.includes(x)
来源：http://kfc.hywenlv.cn

TS:   arr.includes(x)
来源：http://ctt.sysykeji.top

Java: list.contains(x)
来源：http://llr.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://odl.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://ocq.sweek.top

C#:   list.Contains(x)
来源：http://bhr.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://uob.gaohongyu789.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ust.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vby.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xuz.jianghu66.top

TS:   [...arr];
来源：http://cmq.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://ygk.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gxl.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://qhh.sweek.top

C#:   new List<int>(list);
来源：http://nxh.aibaodan.cn

[D23] reduce 累积计算
来源：http://zky.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xxv.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fhm.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://euu.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ler.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ryj.yj20258.top

Go:   // 手写循环
来源：http://van.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cwu.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zdp.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://tuj.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qlo.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lvz.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bfx.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kcp.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uqc.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://drb.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jek.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wcf.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://bqx.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://emx.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://roi.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://srf.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://afo.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://srr.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xdt.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dtj.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ubl.shuidangran.top

[D26] 数组转字符串
来源：http://ajf.uphjek.com

Py:   ", ".join(map(str, arr))
来源：http://cvw.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://pss.hnqzz.top

JS:   arr.join(", ")
来源：http://rny.tarul.cn

TS:   arr.join(", ")
来源：http://chm.zdqjudy.top

Java: String.join(", ", list)
来源：http://xta.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://qyd.0kj1m.cn

Ruby: arr.join(", ")
来源：http://dca.redwolf501.top

C#:   string.Join(", ", list)
来源：http://zsk.shangyingyoupin.top

================================================================================
来源：http://wky.quarkkingdee.top

E. 字符串处理
来源：http://qjw.gotoacloud.top

================================================================================
来源：http://zkn.hnqzz.top

[E01] 拼接字符串
来源：http://prg.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cgz.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uue.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfm.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxk.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hnz.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://osl.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fvw.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ano.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://efe.ybcxt.top

Py:   "ab" * 3
来源：http://oco.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://gbc.yueranfly.top

JS:   "ab".repeat(3)
来源：http://oym.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://xei.xziqi.cn

Java: "ab".repeat(3)
来源：http://xjj.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://zkb.nanxuanxn.top

Ruby: "ab" * 3
来源：http://zbu.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bog.feifeiyinyue.top

[E03] 截取子串
来源：http://znr.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tjx.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uhg.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dre.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://vog.jqgfzy.top

Java: s.substring(1, 4)
来源：http://xyw.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://twv.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://lnj.yueranfly.top

C#:   s.Substring(1, 3)
来源：http://ufh.gzhubu.top

[E04] 查找子串位置
来源：http://ngt.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://rzx.yfazqb.com

PHP:  strpos($s, "x");
来源：http://xnm.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://flm.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://mla.yj20258.top

Java: s.indexOf("x")
来源：http://nog.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://hqo.jinqigfzy.top

Ruby: s.index("x")
来源：http://jjr.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://buj.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mtl.birdmap.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uuz.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mtw.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ckp.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sdt.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uxd.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wkm.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mcq.hesvh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pba.nanxinkj.top

[E06] 替换子串
来源：http://vil.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rbu.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://ccm.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://chc.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://tis.fengsongda.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jco.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uul.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cnu.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://lwo.tian-w.cn

[E07] 按分隔符拆分
来源：http://jkb.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mpw.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fet.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ghx.epnwcf.com

TS:   s.split(",")
来源：http://utv.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://hla.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zns.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://uhp.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qko.yj202588.top

[E08] 数组按分隔符合并
来源：http://hgf.zdbjq.cn

Py:   ",".join(items)
来源：http://lcq.epnwcf.com

PHP:  implode(",", $items);
来源：http://bgu.chenzaomai.com

JS:   items.join(",")
来源：http://jqp.jianghu66.top

TS:   items.join(",")
来源：http://yww.kuanghao11.cn

Java: String.join(",", items)
来源：http://qez.gzhubu.top


<!-- 参考信息 -->