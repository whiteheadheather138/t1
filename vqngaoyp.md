代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://xqg.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://rdv.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://orw.gaohongyu789.top

================================================================================
来源：http://wso.quarkkingdee.top

D. 数组 / 列表 / 集合
来源：http://qqn.jqgufenzy.top

================================================================================
来源：http://qbv.vehdjk.com

[D01] 创建数组 / 列表
来源：http://lxj.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rfo.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ise.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lnj.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bsm.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zzx.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://wtn.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://jxs.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vwh.fktsv.cn

[D02] 追加元素到末尾
来源：http://dzy.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lnp.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nll.daria6918.cn

JS:   arr.push(4);
来源：http://biz.vehdjk.com

TS:   arr.push(4);
来源：http://cgx.ybcxt.top

Java: list.add(4);
来源：http://acx.uphjek.com

Go:   arr = append(arr, 4)
来源：http://aqd.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://ykd.fengsongda.top

C#:   list.Add(4);
来源：http://wph.c1oappe.top

[D03] 在指定位置插入元素
来源：http://ftf.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://icj.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lvc.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zun.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://emm.gotoacloud.top

Java: list.add(0, 0);
来源：http://mxy.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ttd.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pbl.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://nck.guowangkeji.top

[D04] 删除元素
来源：http://fkk.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bpd.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yus.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qoz.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://ljo.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uns.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zxo.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cku.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dpq.gzhubu.top

[D05] 访问与修改元素
来源：http://thi.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rwu.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dli.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nkw.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://xqd.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://qok.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://nxd.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pba.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pbq.bbcook.cn

[D06] 数组长度
来源：http://hdi.jinqigufen.top

Py:   len(arr)
来源：http://kcj.cheryme.top

PHP:  count($arr);
来源：http://hkt.tarul.cn

JS:   arr.length
来源：http://bxr.andypj.xyz

TS:   arr.length
来源：http://yrn.hongshengwenyu.top

Java: list.size();
来源：http://yah.jqgfzy.top

Go:   len(arr)
来源：http://clh.xinyue.icu

Ruby: arr.length; arr.size
来源：http://tej.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://ndd.yfazqb.com

[D07] 切片 / 取子数组
来源：http://nbr.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lcc.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vty.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://xjs.cashguo.top

TS:   arr.slice(1, 4);
来源：http://nvx.pycfn.com

Java: list.subList(1, 4);
来源：http://ute.daria6918.cn

Go:   arr[1:4]
来源：http://ejq.yfazqb.com

Ruby: arr[1, 3]
来源：http://idn.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://tsz.gzhubu.top

[D08] 合并两个数组
来源：http://unq.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://jpu.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://zfm.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bqn.ybcxt.top

TS:   [...a, ...b];
来源：http://iup.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mgq.tarul.cn

Go:   append(a, b...)
来源：http://jsr.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://gtq.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://zyr.jinqigfzy.top

[D09] 排序（升序）
来源：http://zgc.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://wyb.jiagoushi.top

PHP:  sort($arr);
来源：http://rwd.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hal.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hsz.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://teu.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kiv.cqqwz.cn

Ruby: arr.sort
来源：http://ile.kuanghao11.cn

C#:   list.Sort();
来源：http://zsz.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qar.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://okx.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jbr.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ije.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://urn.smart0.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ndj.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://onm.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://arq.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://koa.yanxiufei.cn

[D11] 反转数组
来源：http://ljf.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ktk.hcnkem.com

PHP:  array_reverse($arr);
来源：http://nxi.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tll.jianghu66.top

TS:   [...arr].reverse();
来源：http://qul.snrcjt.cn

Java: Collections.reverse(list);
来源：http://mrc.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://hih.cheryme.top

Ruby: arr.reverse
来源：http://vph.gotoacloud.top

C#:   list.Reverse();
来源：http://wpu.sjlbkw.cn

[D12] 查找元素下标
来源：http://xws.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://mcl.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bbl.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yqz.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xih.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aft.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://vey.wangshuangyany.cn

Ruby: arr.index(x)
来源：http://lis.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://bcy.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://kgl.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cku.dashuyun.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dpz.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://cam.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://wpc.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ucd.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://syu.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://pit.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://shh.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://xcc.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jqv.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dho.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://qqi.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://bik.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ksc.hongshengwenyu.top

Go:   // 手写循环
来源：http://eqn.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://vkq.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://pts.yonumen.top

[D15] 去重
来源：http://bwp.yfazqb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kde.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://kvq.xuanzx.com

JS:   [...new Set(arr)]
来源：http://cak.bjfxy.top

TS:   [...new Set(arr)]
来源：http://fgi.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lcf.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://ejv.ppjwa.cn

Ruby: arr.uniq
来源：http://asc.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://nth.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://fvm.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://moh.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wha.sjlbkw.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rkx.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://why.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fgn.mhx1999.top

Go:   // 手写循环累加
来源：http://ljx.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tmc.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://fup.daria6918.cn

[D17] 最大值与最小值
来源：http://coz.meibo888.top

Py:   max(arr);  min(arr)
来源：http://mal.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://psl.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zbl.hesvh.cn

TS:   Math.max(...arr);
来源：http://xnf.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://whr.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gml.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://mue.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://kdb.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://vro.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rev.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://tyg.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hnp.yj20258.top

TS:   nested.flat();
来源：http://rem.fktsv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iea.daria6918.cn

Go:   // 手写双层循环
来源：http://yum.zdbjq.cn

Ruby: nested.flatten
来源：http://ocw.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ysa.daria6918.cn

[D19] 按字段分组
来源：http://riy.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bln.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ews.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://amu.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jit.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tun.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://khr.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ivm.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zyb.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://aer.yangfankeji.com

Py:   Counter(arr)
来源：http://tnq.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://nms.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nws.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qqt.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tmc.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://bfa.uphjek.com

Ruby: arr.tally
来源：http://tzm.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aac.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://hfy.yueranfly.top

Py:   x in arr
来源：http://wmn.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://obn.zhijiandao.cn

JS:   arr.includes(x)
来源：http://zti.ppjwa.cn

TS:   arr.includes(x)
来源：http://ggv.dashuyun.cn

Java: list.contains(x)
来源：http://mlu.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://fdk.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://jct.kuanghao11.cn

C#:   list.Contains(x)
来源：http://yxx.jiagoushi.top

[D22] 复制数组（避免共享引用）
来源：http://npe.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ccd.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cna.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xdd.fehbvm.com

TS:   [...arr];
来源：http://iuc.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://yjk.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://vtl.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://yuj.yongpay.top

C#:   new List<int>(list);
来源：http://sfy.yuanzhike.top

[D23] reduce 累积计算
来源：http://zod.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hnm.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ygh.jyoumei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://moa.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nxg.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://jhe.ybcxt.top

Go:   // 手写循环
来源：http://kch.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dyk.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qbd.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://cob.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zod.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ybr.nanxuanxn.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dpw.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fuv.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oer.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iht.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://msq.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dul.sweek.top

[D25] Set 集合去重与交并差
来源：http://qib.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pbj.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dae.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kns.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zta.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nso.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cum.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uie.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dvs.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://kra.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://cbh.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://czy.nanxinkj.top

JS:   arr.join(", ")
来源：http://jsh.yfazqb.com

TS:   arr.join(", ")
来源：http://syj.andypj.xyz

Java: String.join(", ", list)
来源：http://hvk.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://lju.cdnleiting.top

Ruby: arr.join(", ")
来源：http://brz.316326.xyz

C#:   string.Join(", ", list)
来源：http://tnr.jqgufenzy.top

================================================================================
来源：http://vbr.zhoulong.xyz

E. 字符串处理
来源：http://pze.ybcxt.top

================================================================================
来源：http://zaw.guowangkeji.top

[E01] 拼接字符串
来源：http://fam.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jeg.yj20258888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://njo.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vjv.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hdh.xuanzx.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ifr.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vgy.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uqn.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xzq.cashguo.top

[E02] 重复字符串
来源：http://vsr.snrcjt.cn

Py:   "ab" * 3
来源：http://jdl.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://tsg.xinyue.icu

JS:   "ab".repeat(3)
来源：http://nwf.tian-w.cn

TS:   "ab".repeat(3)
来源：http://fct.hysaishi.cn

Java: "ab".repeat(3)
来源：http://lsx.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://dtt.zhengqikj.top

Ruby: "ab" * 3
来源：http://cdo.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sbh.yonumen.top

[E03] 截取子串
来源：http://zpa.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wzl.pengpengdd.cyou

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hiy.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://thu.sxryk.cn

TS:   s.slice(1, 4)
来源：http://ppt.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://ouv.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://egn.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dtq.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://mvi.vqdsnc.cn

[E04] 查找子串位置
来源：http://wtz.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://npl.cashguo.top

PHP:  strpos($s, "x");
来源：http://zxa.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qpd.chenzaomai.com

TS:   s.indexOf("x")
来源：http://qvw.daxiang520.top

Java: s.indexOf("x")
来源：http://cvz.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://cso.zhixingplan.top

Ruby: s.index("x")
来源：http://jil.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://mgd.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sjy.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nab.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kdz.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://umk.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://eyd.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mkk.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lvn.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://elf.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xmt.epnwcf.com

[E06] 替换子串
来源：http://jeq.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fkf.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://rji.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://non.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://wax.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mut.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xfs.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://esf.yj202588.top

C#:   s.Replace("a", "b")
来源：http://qjc.gotoacloud.top

[E07] 按分隔符拆分
来源：http://exu.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fhi.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hwn.havefunace.top


<!-- 参考信息 -->