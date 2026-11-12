代发 wailian999

PHP:  // 无重载
来源：http://qsq.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eoc.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://jvi.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vws.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://dmx.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://fzq.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://jnx.cheryme.top

================================================================================
来源：http://fbw.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://zxz.hysaishi.cn

================================================================================
来源：http://fmb.sysykeji.top

[D01] 创建数组 / 列表
来源：http://mcr.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jum.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wvz.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://esi.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wtx.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vqg.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://olk.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://ppq.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sok.xinyue.icu

[D02] 追加元素到末尾
来源：http://ikq.hnqzz.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sgp.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ixu.svipenyu.cn

JS:   arr.push(4);
来源：http://ehy.sjlbkw.cn

TS:   arr.push(4);
来源：http://weu.haohaochexian.top

Java: list.add(4);
来源：http://ndi.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://hij.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://bor.chenzaomai.com

C#:   list.Add(4);
来源：http://ban.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://dtz.hammf.cn

Py:   arr.insert(0, 0)
来源：http://lwr.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dlj.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tfh.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://hqd.hnqzz.top

Java: list.add(0, 0);
来源：http://dlm.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://wwo.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yhg.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://ucc.zhijiandao.cn

[D04] 删除元素
来源：http://crr.gaohongyu789.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mjv.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pth.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ndc.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://fou.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ipz.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xsp.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yso.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zir.sufxvd.cn

[D05] 访问与修改元素
来源：http://zam.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://igf.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ags.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ooq.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cca.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://ank.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://vhd.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ade.jinghuilouyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bhf.tian-w.cn

[D06] 数组长度
来源：http://nde.daxiang520.top

Py:   len(arr)
来源：http://flc.daxiang520.top

PHP:  count($arr);
来源：http://gwl.iojbl.cn

JS:   arr.length
来源：http://lgf.sweek.top

TS:   arr.length
来源：http://ehy.quarkkingdee.top

Java: list.size();
来源：http://lli.nwbrower.top

Go:   len(arr)
来源：http://shb.ivvv.top

Ruby: arr.length; arr.size
来源：http://nav.vehdjk.com

C#:   list.Count;
来源：http://qbj.zycfv.cn

[D07] 切片 / 取子数组
来源：http://rdm.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wbx.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jby.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://amm.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://ttx.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://pgh.sxryk.cn

Go:   arr[1:4]
来源：http://eqj.yueranfly.top

Ruby: arr[1, 3]
来源：http://haj.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://ruh.cashguo.top

[D08] 合并两个数组
来源：http://gtu.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://gzq.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://chn.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hml.tanke756.top

TS:   [...a, ...b];
来源：http://spc.gzhubu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ovk.hongshengwenyu.top

Go:   append(a, b...)
来源：http://bco.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://hkk.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://oiw.svipenyu.cn

[D09] 排序（升序）
来源：http://rrk.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://lwt.jinqigfzy.top

PHP:  sort($arr);
来源：http://tsb.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pgo.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fgf.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fsr.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pep.gotoacloud.top

Ruby: arr.sort
来源：http://iqr.zhongyouzk.top

C#:   list.Sort();
来源：http://itq.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eci.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ouw.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://syt.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://avq.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cmp.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jgs.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://epo.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jik.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zqo.hnqzz.top

[D11] 反转数组
来源：http://qpq.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://uaa.sweek.top

PHP:  array_reverse($arr);
来源：http://exu.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pej.zdqjudy.top

TS:   [...arr].reverse();
来源：http://dfo.hfpthk.cn

Java: Collections.reverse(list);
来源：http://jfh.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://tta.ybcxt.top

Ruby: arr.reverse
来源：http://riz.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://nqs.ivvv.top

[D12] 查找元素下标
来源：http://plf.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://tzm.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://awv.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hlu.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fgm.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gug.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://cik.birdmap.top

Ruby: arr.index(x)
来源：http://rtn.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://tyn.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://txg.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ndh.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xob.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://npb.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://uew.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sbk.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qig.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lcj.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gel.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://xkw.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dnz.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nox.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://xox.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://zdd.daria6918.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mwg.feifeiyinyue.top

Go:   // 手写循环
来源：http://bfw.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bzi.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://eyg.52xcode.cn

[D15] 去重
来源：http://ueb.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xsv.hcnkem.com

PHP:  array_unique($arr);
来源：http://qup.hnqzz.top

JS:   [...new Set(arr)]
来源：http://wox.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://nif.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hir.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://fxa.zhongyouzk.top

Ruby: arr.uniq
来源：http://fdr.pengpengdd.cyou

C#:   list.Distinct().ToList()
来源：http://fzy.sjlbkw.cn

[D16] 求和与平均值
来源：http://cba.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xez.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jya.fehbvm.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vij.52xcode.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ogn.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yzv.vqdsnc.cn

Go:   // 手写循环累加
来源：http://ewa.cdnleiting.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qdj.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://ypq.shuidangran.top

[D17] 最大值与最小值
来源：http://uxj.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://ico.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://cmd.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ohd.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://tks.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://fgu.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pka.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://sjz.tanke756.top

C#:   list.Max();  list.Min()
来源：http://xot.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://xyo.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pov.jlsjyb.cn

PHP:  array_merge(...$nested);
来源：http://dxp.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ipn.wangshuangyany.cn

TS:   nested.flat();
来源：http://xpv.zycfv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bcb.zhengqikj.top

Go:   // 手写双层循环
来源：http://gwt.nanxuanxn.top

Ruby: nested.flatten
来源：http://zbz.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hhb.fktsv.cn

[D19] 按字段分组
来源：http://hpl.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tba.yangfankeji.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ewk.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tdo.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xjy.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://whh.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://udh.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pju.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qwv.sjlbkw.cn

[D20] 统计每个元素出现次数
来源：http://zqk.jlsjyb.cn

Py:   Counter(arr)
来源：http://nmz.zhongyouzk.top

PHP:  array_count_values($arr);
来源：http://tga.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wbm.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gcm.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hkz.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://dnr.tianlin.xyz

Ruby: arr.tally
来源：http://gqf.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jyj.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://rki.fengsongda.top

Py:   x in arr
来源：http://dfr.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://gyb.gogol.net.cn

JS:   arr.includes(x)
来源：http://otv.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://uby.nanxuanxn.top

Java: list.contains(x)
来源：http://fuu.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://qgd.daria6918.cn

Ruby: arr.include?(x)
来源：http://fcr.daxiang520.top

C#:   list.Contains(x)
来源：http://ynh.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://azm.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nuf.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dma.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://whm.52xcode.cn

TS:   [...arr];
来源：http://qdn.daxiang520.top

Java: new ArrayList<>(list);
来源：http://kvt.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gry.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://lyh.chenlongwang.top

C#:   new List<int>(list);
来源：http://wnt.dashuyun.cn

[D23] reduce 累积计算
来源：http://ojb.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zgg.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mqr.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wba.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://smy.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://omv.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://xpp.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uii.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sms.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://pdd.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lwx.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kup.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://opo.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bbn.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vvx.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vpm.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xgc.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://omb.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://hke.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uyb.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wyb.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fxw.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://psy.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mph.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zeg.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gbb.fengsongda.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rkh.yongpay.top

[D26] 数组转字符串
来源：http://lcg.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://qmw.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://hss.yuxming.cn

JS:   arr.join(", ")
来源：http://nmz.jqgfzy.top

TS:   arr.join(", ")
来源：http://pgb.zhoulong.xyz

Java: String.join(", ", list)
来源：http://rsp.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://jkb.shzxlz.cn

Ruby: arr.join(", ")
来源：http://aev.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://dft.tian-w.cn

================================================================================
来源：http://vdz.smart0.xyz

E. 字符串处理
来源：http://ski.cqqwz.cn

================================================================================
来源：http://tkq.sjlbkw.cn

[E01] 拼接字符串
来源：http://bje.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vgp.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tzb.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hss.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oqo.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pky.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iha.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ggm.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cbg.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://xqi.aizwys.cn

Py:   "ab" * 3
来源：http://jdt.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://gbj.sysykeji.top

JS:   "ab".repeat(3)
来源：http://ios.cashguo.top

TS:   "ab".repeat(3)
来源：http://yxk.hammf.cn

Java: "ab".repeat(3)
来源：http://nvj.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://dgs.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://afp.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cmy.redwolf501.top

[E03] 截取子串
来源：http://wnd.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tpb.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pwo.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nam.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://thn.yueranfly.top

Java: s.substring(1, 4)
来源：http://czu.ehwqpu.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ymf.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://gjt.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://mrb.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://ukl.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://evm.fzhhl.top

PHP:  strpos($s, "x");
来源：http://nyt.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qqu.hysaishi.cn

TS:   s.indexOf("x")
来源：http://arm.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://lfg.yj202588.top

Go:   strings.Index(s, "x")
来源：http://ggf.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://djw.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://mqc.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://slr.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://frl.tarul.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rgc.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tkj.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://xas.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oox.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yak.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rxk.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fjc.tianlin.xyz

[E06] 替换子串
来源：http://qcz.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iig.shanyushiyangtech.top

PHP:  str_replace("a", "b", $s);
来源：http://ogy.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qak.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://czm.iojbl.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zif.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yru.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gtp.9152youxi.cn


<!-- 参考信息 -->