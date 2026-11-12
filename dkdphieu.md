代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://abe.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dph.tanke756.top

Java: // 无解构
来源：http://xpn.wangdashe.top

Go:   // 无解构
来源：http://nhy.cdnleiting.top

Ruby: a, b = pair
来源：http://rvz.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://uau.xinyue.icu

[C16] 函数 / 方法重载
来源：http://yxn.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hzx.ybcxt.top

PHP:  // 无重载
来源：http://oie.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://yjq.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://pnx.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wgi.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://bwr.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://xrx.tanke756.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://osp.hywenlv.cn

================================================================================
来源：http://joc.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://och.xinyue.icu

================================================================================
来源：http://icv.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://std.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ovs.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zwe.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zlc.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pkc.pycfn.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zpo.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://hqv.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://arp.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gfv.dianchejie.cn

[D02] 追加元素到末尾
来源：http://tbo.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://drg.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dyf.xziqi.cn

JS:   arr.push(4);
来源：http://kkv.fzhhl.top

TS:   arr.push(4);
来源：http://zea.fehbvm.com

Java: list.add(4);
来源：http://jpr.xingfuxueyuan.xyz

Go:   arr = append(arr, 4)
来源：http://hhj.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://kxs.bbcook.cn

C#:   list.Add(4);
来源：http://uba.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://voe.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://qev.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://srl.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://huf.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://cxf.chenzaomai.com

Java: list.add(0, 0);
来源：http://khl.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cio.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://syn.fehbvm.com

C#:   list.Insert(0, 0);
来源：http://ggm.jianghu66.top

[D04] 删除元素
来源：http://ifu.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cfs.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qey.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dpo.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://vvy.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yrf.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mgn.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://erj.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bve.zhoulong.xyz

[D05] 访问与修改元素
来源：http://xqf.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wpo.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tza.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tss.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://nld.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://rmh.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://yzt.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mnm.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qvy.birdmap.top

[D06] 数组长度
来源：http://gta.yj20258888.top

Py:   len(arr)
来源：http://mtv.fktsv.cn

PHP:  count($arr);
来源：http://nvr.zhengqikj.top

JS:   arr.length
来源：http://waz.tanke756.top

TS:   arr.length
来源：http://ynl.tarul.cn

Java: list.size();
来源：http://qbb.ywan-chungtsiang.top

Go:   len(arr)
来源：http://cvi.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://kyc.yfazqb.com

C#:   list.Count;
来源：http://hvs.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://hxh.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tms.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://rwq.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://bdz.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://pyr.yfazqb.com

Java: list.subList(1, 4);
来源：http://lyb.feifeiyinyue.top

Go:   arr[1:4]
来源：http://oye.tanke756.top

Ruby: arr[1, 3]
来源：http://xul.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://izn.pengpengdd.cyou

[D08] 合并两个数组
来源：http://zel.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://ghl.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://cey.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tau.ydzc1.top

TS:   [...a, ...b];
来源：http://rdv.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://omb.zhixingplan.top

Go:   append(a, b...)
来源：http://hzo.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://sgu.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://nkp.zhengqikj.top

[D09] 排序（升序）
来源：http://ykb.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://utl.jyoumei.cn

PHP:  sort($arr);
来源：http://zmg.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qou.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fjt.52xcode.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xzk.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hvg.yj20258888.top

Ruby: arr.sort
来源：http://woq.zhiwuduotai.top

C#:   list.Sort();
来源：http://ykk.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ywd.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://krv.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sfn.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://exb.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wrs.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://asn.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xix.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://abj.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xgd.fktsv.cn

[D11] 反转数组
来源：http://oqh.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://zuf.meibo888.top

PHP:  array_reverse($arr);
来源：http://rov.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gwz.redwolf501.top

TS:   [...arr].reverse();
来源：http://ort.redwolf501.top

Java: Collections.reverse(list);
来源：http://cuw.aizwys.cn

Go:   slices.Reverse(arr)
来源：http://uel.gaohongyu789.top

Ruby: arr.reverse
来源：http://ayt.guowangkeji.top

C#:   list.Reverse();
来源：http://sda.ehwqpu.com

[D12] 查找元素下标
来源：http://cyq.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://ysf.hammf.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ccl.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vwh.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ftd.smart0.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oem.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://drc.ydjk.org.cn

Ruby: arr.index(x)
来源：http://voz.bjfxy.top

C#:   list.IndexOf(x);
来源：http://smd.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://ysw.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lec.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ztm.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://nds.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://wxk.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ekd.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nzo.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://bnt.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wbe.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://fqz.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vid.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qhq.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://nwr.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://ryq.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yki.hammf.cn

Go:   // 手写循环
来源：http://rzu.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://acv.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sox.hnqzz.top

[D15] 去重
来源：http://szm.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mfw.shuidangran.top

PHP:  array_unique($arr);
来源：http://mqu.bjfxy.top

JS:   [...new Set(arr)]
来源：http://qzi.hnqzz.top

TS:   [...new Set(arr)]
来源：http://rnt.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zrd.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://miw.hfpthk.cn

Ruby: arr.uniq
来源：http://yrz.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://sby.xuanzx.com

[D16] 求和与平均值
来源：http://lww.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qin.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jww.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uyp.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uom.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://urc.fzhhl.top

Go:   // 手写循环累加
来源：http://dxy.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eoq.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://pbx.zdqjudy.top

[D17] 最大值与最小值
来源：http://tor.hammf.cn

Py:   max(arr);  min(arr)
来源：http://are.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://bia.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://usj.chenzaomai.com

TS:   Math.max(...arr);
来源：http://tfc.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tun.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://upi.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://hhn.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://ufo.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://bbh.ywan-chungtsiang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iwv.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://rmj.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bou.iojbl.cn

TS:   nested.flat();
来源：http://qxg.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://edt.aibaodan.cn

Go:   // 手写双层循环
来源：http://zas.chenzaomai.com

Ruby: nested.flatten
来源：http://atr.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ugv.jqgfzy.top

[D19] 按字段分组
来源：http://vwv.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wma.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zse.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qoa.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vxw.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mlp.birdmap.top

Go:   // 手写 map[string][]T
来源：http://jgb.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://udg.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qnn.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://akj.hammf.cn

Py:   Counter(arr)
来源：http://qsy.fengsongda.top

PHP:  array_count_values($arr);
来源：http://rba.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ial.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qwx.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xax.cashguo.top

Go:   // 手写 map[T]int
来源：http://kku.zdqjudy.top

Ruby: arr.tally
来源：http://idf.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hgu.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://rgh.ehwqpu.com

Py:   x in arr
来源：http://wgj.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://gsz.zycfv.cn

JS:   arr.includes(x)
来源：http://xof.gzhubu.top

TS:   arr.includes(x)
来源：http://xdn.nwbrower.top

Java: list.contains(x)
来源：http://gfe.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://elb.iojbl.cn

Ruby: arr.include?(x)
来源：http://dnb.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://gjb.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://vdn.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qip.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qtp.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jyb.snrcjt.cn

TS:   [...arr];
来源：http://jep.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://xsp.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://gln.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://kgs.yuxming.cn

C#:   new List<int>(list);
来源：http://mue.xuanzx.com

[D23] reduce 累积计算
来源：http://gfq.yvedp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rka.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ysv.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rlt.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jga.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://byq.zdqjudy.top

Go:   // 手写循环
来源：http://fdn.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iby.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ysz.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://apz.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hao.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cdm.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ioq.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nnh.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://orr.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hea.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://smn.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dsl.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://dav.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gjq.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fgh.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://doh.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ntl.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nkk.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lzd.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ixh.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ouz.gotoacloud.top

[D26] 数组转字符串
来源：http://hbw.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://zsh.uphjek.com

PHP:  implode(", ", $arr);
来源：http://pxy.sufxvd.cn

JS:   arr.join(", ")
来源：http://rmt.guowangkeji.top

TS:   arr.join(", ")
来源：http://wpq.zdbjq.cn

Java: String.join(", ", list)
来源：http://hrj.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://cnb.aizwys.cn

Ruby: arr.join(", ")
来源：http://kwc.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://bvd.hysaishi.cn

================================================================================
来源：http://mla.vqdsnc.cn

E. 字符串处理
来源：http://ank.nanxuanxn.top

================================================================================
来源：http://zgy.iojbl.cn

[E01] 拼接字符串
来源：http://bra.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yvo.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lxo.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yri.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vba.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gfe.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nny.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wdh.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kfx.hysaishi.cn

[E02] 重复字符串
来源：http://nhu.havefunace.top

Py:   "ab" * 3
来源：http://zzw.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://zkv.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://ovh.hnqzz.top

TS:   "ab".repeat(3)
来源：http://uhr.yvedp.cn

Java: "ab".repeat(3)
来源：http://zlr.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://dfw.andypj.xyz

Ruby: "ab" * 3
来源：http://xbc.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oth.svipenyu.cn

[E03] 截取子串
来源：http://ofv.svipenyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jup.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wjm.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wei.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://iep.gzhubu.top

Java: s.substring(1, 4)
来源：http://lmh.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://arq.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://tal.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://zpe.wangdashe.top

[E04] 查找子串位置
来源：http://sof.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://mdm.cheryme.top

PHP:  strpos($s, "x");
来源：http://nsj.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xmr.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://qqf.aibaodan.cn

Java: s.indexOf("x")
来源：http://kol.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://wmm.meibo888.top

Ruby: s.index("x")
来源：http://tvx.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://rry.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cum.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://juu.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hpn.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yaj.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://hrr.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qvk.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://irt.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ubs.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://piq.tanke756.top


<!-- 参考信息 -->