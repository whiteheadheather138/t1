代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qva.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cwg.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uba.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zmx.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://fdq.redwolf501.top

Ruby: arr = [1, 2, 3]
来源：http://dvx.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cvq.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://xbd.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ydr.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jpo.jianghu66.top

JS:   arr.push(4);
来源：http://fle.daria6918.cn

TS:   arr.push(4);
来源：http://yhp.epnwcf.com

Java: list.add(4);
来源：http://skz.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://tbj.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://thj.hcnkem.com

C#:   list.Add(4);
来源：http://hrp.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://pmb.yj202588.top

Py:   arr.insert(0, 0)
来源：http://hyj.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qha.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uty.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://zid.kuanghao11.cn

Java: list.add(0, 0);
来源：http://xmh.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://keu.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wav.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://lnz.zhaomingkeji.xyz

[D04] 删除元素
来源：http://vwm.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hoj.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lqa.wangdashe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ywi.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://hvj.hywenlv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uts.yonumen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kfl.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fvh.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jsv.xziqi.cn

[D05] 访问与修改元素
来源：http://yii.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nuf.hnxiangtu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pbk.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wyx.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://mde.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://bav.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://zld.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fou.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xkt.aibaodan.cn

[D06] 数组长度
来源：http://mbk.chenjidiqi.icu

Py:   len(arr)
来源：http://olj.jianghu66.top

PHP:  count($arr);
来源：http://gbv.c1oappe.top

JS:   arr.length
来源：http://ses.yongpay.top

TS:   arr.length
来源：http://ans.quarkkingdee.top

Java: list.size();
来源：http://gao.sweek.top

Go:   len(arr)
来源：http://ksk.iojbl.cn

Ruby: arr.length; arr.size
来源：http://wem.yangfankeji.com

C#:   list.Count;
来源：http://vns.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://wiu.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iff.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://pdn.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://zbz.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://qis.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://axb.aibaodan.cn

Go:   arr[1:4]
来源：http://xva.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://gbz.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://eja.zdqjudy.top

[D08] 合并两个数组
来源：http://eyu.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://gdh.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://qfq.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://egp.tianlin.xyz

TS:   [...a, ...b];
来源：http://wzb.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://koo.daria6918.cn

Go:   append(a, b...)
来源：http://yqz.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://ofb.sweek.top

C#:   a.Concat(b).ToList()
来源：http://uwr.zhiwuduotai.top

[D09] 排序（升序）
来源：http://gbr.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://kyr.fktsv.cn

PHP:  sort($arr);
来源：http://yed.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://isw.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gte.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pov.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kef.wangshuangyany.cn

Ruby: arr.sort
来源：http://yqj.cashguo.top

C#:   list.Sort();
来源：http://qir.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://txa.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pqk.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ewl.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ewq.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pdu.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ago.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gha.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://web.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cbg.zhengqikj.top

[D11] 反转数组
来源：http://iug.sufxvd.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hwd.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://rqa.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://idx.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://qjc.c1oappe.top

Java: Collections.reverse(list);
来源：http://igt.pycfn.com

Go:   slices.Reverse(arr)
来源：http://zfe.smart0.xyz

Ruby: arr.reverse
来源：http://cab.tian-w.cn

C#:   list.Reverse();
来源：http://tni.epnwcf.com

[D12] 查找元素下标
来源：http://uof.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://fjr.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://emx.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vie.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vam.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jim.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://hwk.wangdashe.top

Ruby: arr.index(x)
来源：http://wut.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://iwk.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://ksr.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dto.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wgh.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://yqz.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://izw.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tmk.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hbf.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ied.zhixingplan.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yqs.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://pgh.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://akw.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qrv.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://ari.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://fet.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qkt.sxryk.cn

Go:   // 手写循环
来源：http://wkk.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://klc.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://joi.jinghuilouyu.cn

[D15] 去重
来源：http://eth.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fug.ivvv.top

PHP:  array_unique($arr);
来源：http://eon.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://vmt.yongpay.top

TS:   [...new Set(arr)]
来源：http://uuw.xylfe.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hye.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://ibm.gogol.net.cn

Ruby: arr.uniq
来源：http://azd.cheryme.top

C#:   list.Distinct().ToList()
来源：http://jan.ppjwa.cn

[D16] 求和与平均值
来源：http://xyu.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://joo.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qwo.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://msx.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://otm.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ibu.dianchejie.cn

Go:   // 手写循环累加
来源：http://rry.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pep.daxiang520.top

C#:   list.Sum();  list.Average()
来源：http://mln.fanxiaobao.xyz

[D17] 最大值与最小值
来源：http://enq.meibo888.top

Py:   max(arr);  min(arr)
来源：http://kho.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://cth.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qdq.shzxlz.cn

TS:   Math.max(...arr);
来源：http://dwl.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vuc.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vup.316326.xyz

Ruby: arr.max;  arr.min
来源：http://ukc.yonumen.top

C#:   list.Max();  list.Min()
来源：http://bhh.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://rxl.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xnh.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://ngb.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zof.dashuyun.cn

TS:   nested.flat();
来源：http://gge.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://thc.wangdashe.top

Go:   // 手写双层循环
来源：http://lll.chenlongwang.top

Ruby: nested.flatten
来源：http://yti.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bau.jqgfzy.top

[D19] 按字段分组
来源：http://flx.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ybz.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kkg.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://afe.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zfy.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gkl.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://fxn.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wgt.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mkz.cashguo.top

[D20] 统计每个元素出现次数
来源：http://xrm.sufxvd.cn

Py:   Counter(arr)
来源：http://mze.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://sqg.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://noe.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cuy.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ink.cdnleiting.top

Go:   // 手写 map[T]int
来源：http://xgu.haohaochexian.top

Ruby: arr.tally
来源：http://srt.yuanzhike.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://onz.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://vpu.xziqi.cn

Py:   x in arr
来源：http://dzt.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://iwc.aibaodan.cn

JS:   arr.includes(x)
来源：http://vqy.bjfxy.top

TS:   arr.includes(x)
来源：http://zkl.gogol.net.cn

Java: list.contains(x)
来源：http://jca.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://les.cqqwz.cn

Ruby: arr.include?(x)
来源：http://kmm.jiagoushi.top

C#:   list.Contains(x)
来源：http://qnn.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://zjz.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gbj.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tjk.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qfx.feifeiyinyue.top

TS:   [...arr];
来源：http://wvq.c1oappe.top

Java: new ArrayList<>(list);
来源：http://gzv.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bqn.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://orv.316326.xyz

C#:   new List<int>(list);
来源：http://vai.yj202588.top

[D23] reduce 累积计算
来源：http://meo.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cbo.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://orc.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mce.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bvo.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oav.meibo888.top

Go:   // 手写循环
来源：http://svu.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fjp.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zem.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://mhf.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iop.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kbu.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yfd.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cgj.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://spt.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hhd.uphjek.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://izf.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ppa.uphjek.com

[D25] Set 集合去重与交并差
来源：http://mrx.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zpg.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pfg.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wob.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zpl.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jxh.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tvk.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rdt.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://exv.zhengqikj.top

[D26] 数组转字符串
来源：http://afh.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://yfv.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://lzq.gaohongyu789.top

JS:   arr.join(", ")
来源：http://egh.9152youxi.cn

TS:   arr.join(", ")
来源：http://zai.yvedp.cn

Java: String.join(", ", list)
来源：http://eyg.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://xlq.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://tbe.daxiang520.top

C#:   string.Join(", ", list)
来源：http://zyz.ctjpmb.com

================================================================================
来源：http://vtp.uphjek.com

E. 字符串处理
来源：http://wwg.tian-w.cn

================================================================================
来源：http://qej.aizwys.cn

[E01] 拼接字符串
来源：http://wwh.daria6918.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gmg.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gkh.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hcp.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aag.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uba.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ynw.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fri.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oxg.pengpengdd.cyou

[E02] 重复字符串
来源：http://dsk.zhijiandao.cn

Py:   "ab" * 3
来源：http://jep.tanke756.top

PHP:  str_repeat("ab", 3);
来源：http://bkg.hnqzz.top

JS:   "ab".repeat(3)
来源：http://ylr.yj202588.top

TS:   "ab".repeat(3)
来源：http://jzh.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://lkl.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://aql.sufxvd.cn

Ruby: "ab" * 3
来源：http://ond.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jnq.cdnleiting.top

[E03] 截取子串
来源：http://zpf.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://the.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dbe.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eie.kuanghao11.cn

TS:   s.slice(1, 4)
来源：http://oql.birdmap.top

Java: s.substring(1, 4)
来源：http://arb.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mhc.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://sik.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://erm.guowangkeji.top

[E04] 查找子串位置
来源：http://rco.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://hmq.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://eic.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wev.52xcode.cn

TS:   s.indexOf("x")
来源：http://vdd.zycfv.cn

Java: s.indexOf("x")
来源：http://tyx.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://tlq.jianghu66.top

Ruby: s.index("x")
来源：http://avz.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://zli.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://flr.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ynp.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hbt.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fyh.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://apz.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://exg.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yjq.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://okh.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gjq.quarkkingdee.top

[E06] 替换子串
来源：http://qck.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nar.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://esi.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zav.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://ugd.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xzq.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ykm.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lil.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://nji.gotoacloud.top

[E07] 按分隔符拆分
来源：http://pjm.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lgf.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zdj.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tbi.aizwys.cn

TS:   s.split(",")
来源：http://rvh.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://txh.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yzk.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://sym.hywenlv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rih.yfazqb.com

[E08] 数组按分隔符合并
来源：http://quj.epnwcf.com

Py:   ",".join(items)
来源：http://zba.shzxlz.cn


<!-- 参考信息 -->