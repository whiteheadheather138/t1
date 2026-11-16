代发 wailian999

D. 数组 / 列表 / 集合
来源：http://tvf.shzxlz.cn

================================================================================
来源：http://ntq.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://qxf.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://okh.pycfn.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://afg.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wcy.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mxb.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fsf.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://aut.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://gzo.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gqp.chenlongwang.top

[D02] 追加元素到末尾
来源：http://mdk.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qxr.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tml.sufxvd.cn

JS:   arr.push(4);
来源：http://nlt.xuetiantiany.cn

TS:   arr.push(4);
来源：http://gbj.hesvh.cn

Java: list.add(4);
来源：http://qvg.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://jfw.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://geu.hnxiangtu.top

C#:   list.Add(4);
来源：http://dxs.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://rhl.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://nsr.hfpthk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tze.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ihi.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://apt.kuanghao11.cn

Java: list.add(0, 0);
来源：http://ojt.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mcj.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dlh.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://sqv.ivvv.top

[D04] 删除元素
来源：http://urk.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yll.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://inc.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hqo.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://wbw.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wmk.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rxf.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sxv.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mnc.cashguo.top

[D05] 访问与修改元素
来源：http://zeo.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sqr.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vlc.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lvy.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://fad.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://vbn.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://yjc.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nkr.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zss.ywan-chungtsiang.top

[D06] 数组长度
来源：http://zjm.jqgfzy.top

Py:   len(arr)
来源：http://aio.dianchejie.cn

PHP:  count($arr);
来源：http://tlh.xylfe.cn

JS:   arr.length
来源：http://qyr.316326.xyz

TS:   arr.length
来源：http://cdy.zhiwuduotai.top

Java: list.size();
来源：http://wog.hesvh.cn

Go:   len(arr)
来源：http://tuh.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://ckq.xinyue.icu

C#:   list.Count;
来源：http://mlf.zycfv.cn

[D07] 切片 / 取子数组
来源：http://jqf.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iyq.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://gza.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://hmj.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://jen.nwbrower.top

Java: list.subList(1, 4);
来源：http://myo.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://eow.shangyingyoupin.top

Ruby: arr[1, 3]
来源：http://jof.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://lzo.ctjpmb.com

[D08] 合并两个数组
来源：http://ygw.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://opo.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://guy.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cuz.yj202588.top

TS:   [...a, ...b];
来源：http://mhd.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ggs.fengsongda.top

Go:   append(a, b...)
来源：http://iyl.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://vho.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://kxp.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://anl.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://sno.cashguo.top

PHP:  sort($arr);
来源：http://vmi.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tmw.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://clc.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uxv.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sls.feifeiyinyue.top

Ruby: arr.sort
来源：http://yes.yj20258888.top

C#:   list.Sort();
来源：http://lnb.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://agk.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qcr.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eaz.fehbvm.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://esc.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oui.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://npr.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://auy.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uhm.aibaodan.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vvb.zhengqikj.top

[D11] 反转数组
来源：http://qbr.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zgq.hnqzz.top

PHP:  array_reverse($arr);
来源：http://gdz.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uyu.hnqzz.top

TS:   [...arr].reverse();
来源：http://mcz.jinqigufen.top

Java: Collections.reverse(list);
来源：http://wbj.chenlongwang.top

Go:   slices.Reverse(arr)
来源：http://fhr.yj20258.top

Ruby: arr.reverse
来源：http://vxm.nanxinkj.top

C#:   list.Reverse();
来源：http://dgm.epnwcf.com

[D12] 查找元素下标
来源：http://tqm.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://iij.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jtm.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lel.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fwh.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hcp.yangfankeji.com

Go:   slices.Index(arr, x)
来源：http://qbf.hnqzz.top

Ruby: arr.index(x)
来源：http://fns.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://xsn.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://pwo.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qru.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mvv.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://fqu.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://ytn.aizwys.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fal.svipenyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ulh.cashguo.top

Ruby: arr.select { |x| x > 3 }
来源：http://adp.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iqf.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://zjx.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ssi.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dbo.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://yva.pycfn.com

TS:   arr.map(x => x * 2)
来源：http://kfv.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gru.hywenlv.cn

Go:   // 手写循环
来源：http://kao.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://fyh.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pvq.redwolf501.top

[D15] 去重
来源：http://ioi.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jhx.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://nfy.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://dbk.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://boz.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://idx.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dze.hcnkem.com

Ruby: arr.uniq
来源：http://plf.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://aud.redwolf501.top

[D16] 求和与平均值
来源：http://dxp.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cjr.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wem.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://syp.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rkw.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jyq.ppjwa.cn

Go:   // 手写循环累加
来源：http://igr.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://khl.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://rsw.zycfv.cn

[D17] 最大值与最小值
来源：http://nxn.uphjek.com

Py:   max(arr);  min(arr)
来源：http://fyu.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://lny.hcnkem.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yqs.ppjwa.cn

TS:   Math.max(...arr);
来源：http://ohw.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://wee.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ymg.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://mxj.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://byo.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://vxm.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qpj.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://zjq.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zxs.sjlbkw.cn

TS:   nested.flat();
来源：http://nib.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uid.yuanzhike.top

Go:   // 手写双层循环
来源：http://vqo.cucudq.cn

Ruby: nested.flatten
来源：http://wwn.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://xzl.xuanzx.com

[D19] 按字段分组
来源：http://xto.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oji.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bln.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vsv.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vdo.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zrg.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://jfc.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gfp.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dbw.havefunace.top

[D20] 统计每个元素出现次数
来源：http://sej.aizwys.cn

Py:   Counter(arr)
来源：http://gvi.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://dip.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mfr.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wsa.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qiz.gaohongyu789.top

Go:   // 手写 map[T]int
来源：http://dey.aizwys.cn

Ruby: arr.tally
来源：http://ync.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gta.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://tfe.kuanghao11.cn

Py:   x in arr
来源：http://iun.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://cgc.daria6918.cn

JS:   arr.includes(x)
来源：http://shz.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://btq.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://zol.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://enn.yuanzhike.top

Ruby: arr.include?(x)
来源：http://dnl.aibaodan.cn

C#:   list.Contains(x)
来源：http://hpd.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://nat.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uny.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qyd.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dlg.dianchejie.cn

TS:   [...arr];
来源：http://xzj.xuanzx.com

Java: new ArrayList<>(list);
来源：http://kgv.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fao.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://cyc.xinyue.icu

C#:   new List<int>(list);
来源：http://zlz.yj202588.top

[D23] reduce 累积计算
来源：http://pbo.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yen.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://faz.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rmw.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nyy.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://abl.jqgufenzy.top

Go:   // 手写循环
来源：http://gyx.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oig.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://igt.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://udk.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nxc.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pln.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tef.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gpb.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xiy.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rrb.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cbz.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ucy.hnqzz.top

[D25] Set 集合去重与交并差
来源：http://vib.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nro.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://clf.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://miy.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sso.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hzk.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qln.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aun.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rbw.yfazqb.com

[D26] 数组转字符串
来源：http://ltb.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://zng.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://mac.fktsv.cn

JS:   arr.join(", ")
来源：http://mpp.hesvh.cn

TS:   arr.join(", ")
来源：http://qvk.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://vak.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://qfk.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://rtc.cucudq.cn

C#:   string.Join(", ", list)
来源：http://dqg.nwbrower.top

================================================================================
来源：http://zdv.wangshuangyany.cn

E. 字符串处理
来源：http://wnz.snrcjt.cn

================================================================================
来源：http://zue.pycfn.com

[E01] 拼接字符串
来源：http://srt.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uqu.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pxj.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ndw.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ajj.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cul.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ddr.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gbn.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mpl.yuanzhike.top

[E02] 重复字符串
来源：http://lew.jlsjyb.cn

Py:   "ab" * 3
来源：http://ohu.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://enr.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://rlk.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://ldq.52xcode.cn

Java: "ab".repeat(3)
来源：http://odc.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://fdh.guannengcc.top

Ruby: "ab" * 3
来源：http://tbq.chenjidiqi.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://raq.sufxvd.cn

[E03] 截取子串
来源：http://tzw.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://suf.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qjs.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iim.ivvv.top

TS:   s.slice(1, 4)
来源：http://wjx.hammf.cn

Java: s.substring(1, 4)
来源：http://lxg.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jso.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://qlz.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://tif.andypj.xyz

[E04] 查找子串位置
来源：http://ehv.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://kjy.zycfv.cn

PHP:  strpos($s, "x");
来源：http://cwc.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://srj.wangdashe.top

TS:   s.indexOf("x")
来源：http://ddf.birdmap.top

Java: s.indexOf("x")
来源：http://kbd.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://gfg.hnxiangtu.top

Ruby: s.index("x")
来源：http://nnv.zycfv.cn

C#:   s.IndexOf("x")
来源：http://lkz.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://dem.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cpe.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mun.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tul.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://efo.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jwy.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qty.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pjn.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gko.shanyushiyangkeji.top

[E06] 替换子串
来源：http://ysg.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rfe.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://glm.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wpd.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://ssf.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dev.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://odg.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wnn.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://wxq.hesvh.cn

[E07] 按分隔符拆分
来源：http://duc.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://twf.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tkm.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zor.zhijiandao.cn

TS:   s.split(",")
来源：http://uxx.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://yyv.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iyy.fanxiaobao.xyz


<!-- 参考信息 -->