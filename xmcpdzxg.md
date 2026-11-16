代发 wailian999

Ruby: a, b = pair
来源：http://irj.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://tfj.hesvh.cn

[C16] 函数 / 方法重载
来源：http://bte.zhiwuduotai.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://muh.gotoacloud.top

PHP:  // 无重载
来源：http://zcf.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://srp.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://wzp.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://pww.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://ngf.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://spy.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ipw.yj20258888.top

================================================================================
来源：http://gau.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://oxh.xingfuxueyuan.xyz

================================================================================
来源：http://qyy.bjfxy.top

[D01] 创建数组 / 列表
来源：http://qsw.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mmu.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ppq.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mby.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xmu.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ikm.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://hce.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://def.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zgo.hesvh.cn

[D02] 追加元素到末尾
来源：http://rph.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vvy.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pxx.yongpay.top

JS:   arr.push(4);
来源：http://aje.gogol.net.cn

TS:   arr.push(4);
来源：http://lwk.zycfv.cn

Java: list.add(4);
来源：http://yqs.gogol.net.cn

Go:   arr = append(arr, 4)
来源：http://nda.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://nxu.feifeiyinyue.top

C#:   list.Add(4);
来源：http://chx.hcnkem.com

[D03] 在指定位置插入元素
来源：http://wgf.uphjek.com

Py:   arr.insert(0, 0)
来源：http://wko.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fhj.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vle.fanxiaobao.xyz

TS:   arr.splice(0, 0, 0);
来源：http://gro.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://woc.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iux.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kof.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://lzo.quarkkingdee.top

[D04] 删除元素
来源：http://jki.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://slw.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bhr.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ifh.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://yzp.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ofo.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://stm.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nqg.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bdt.zdqjudy.top

[D05] 访问与修改元素
来源：http://hee.havefunace.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oun.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kml.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rby.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://xme.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://iap.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://xet.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vfg.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rfy.ivvv.top

[D06] 数组长度
来源：http://hbk.jianghu66.top

Py:   len(arr)
来源：http://ieo.tarul.cn

PHP:  count($arr);
来源：http://frp.ydjk.org.cn

JS:   arr.length
来源：http://gvp.zycfv.cn

TS:   arr.length
来源：http://fuj.zhiwuduotai.top

Java: list.size();
来源：http://akn.hysaishi.cn

Go:   len(arr)
来源：http://pfb.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://bro.nwbrower.top

C#:   list.Count;
来源：http://kfk.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://gfd.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lfv.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://txq.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://tus.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://lwg.yuxming.cn

Java: list.subList(1, 4);
来源：http://czf.jqgufenzy.top

Go:   arr[1:4]
来源：http://los.zycfv.cn

Ruby: arr[1, 3]
来源：http://eeh.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://pzo.shzxlz.cn

[D08] 合并两个数组
来源：http://efo.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://ead.iojbl.cn

PHP:  array_merge($a, $b);
来源：http://qvm.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jsq.gotoacloud.top

TS:   [...a, ...b];
来源：http://uss.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pvw.yangfankeji.com

Go:   append(a, b...)
来源：http://utv.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://ylg.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://zhx.yongpay.top

[D09] 排序（升序）
来源：http://vsg.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://amf.0kj1m.cn

PHP:  sort($arr);
来源：http://nbb.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uyl.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://qfd.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://nvd.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kna.yuxming.cn

Ruby: arr.sort
来源：http://abm.birdmap.top

C#:   list.Sort();
来源：http://czy.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rlx.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ppb.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fcj.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vdr.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://inv.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hpd.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://osp.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jai.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zev.uphjek.com

[D11] 反转数组
来源：http://ais.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ujr.zycfv.cn

PHP:  array_reverse($arr);
来源：http://uwe.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dmo.iojbl.cn

TS:   [...arr].reverse();
来源：http://xbh.tianlin.xyz

Java: Collections.reverse(list);
来源：http://ped.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://mtk.xinyue.icu

Ruby: arr.reverse
来源：http://cnp.cucudq.cn

C#:   list.Reverse();
来源：http://iiy.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://tpf.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://tdu.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wpl.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ugt.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aoq.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ued.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://fad.xuanzx.com

Ruby: arr.index(x)
来源：http://tge.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://lgy.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://ils.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cyy.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vju.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://mzz.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://ghl.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wpv.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yye.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://qnv.ivvv.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kbf.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://ysv.zdqjudy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kos.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://enq.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://afj.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://vtf.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lte.xuetiantiany.cn

Go:   // 手写循环
来源：http://loi.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://ytc.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xql.aizwys.cn

[D15] 去重
来源：http://wpa.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jbc.yuanzhike.top

PHP:  array_unique($arr);
来源：http://qka.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://okg.uphjek.com

TS:   [...new Set(arr)]
来源：http://pnt.hammf.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gan.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://odw.hnxiangtu.top

Ruby: arr.uniq
来源：http://ixu.havefunace.top

C#:   list.Distinct().ToList()
来源：http://vog.ppjwa.cn

[D16] 求和与平均值
来源：http://qyx.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cfv.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://btk.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aco.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gsc.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pug.vehdjk.com

Go:   // 手写循环累加
来源：http://sdq.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yik.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://due.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://qvd.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://xbh.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://yml.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://leb.jyoumei.cn

TS:   Math.max(...arr);
来源：http://mnx.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://nln.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lvl.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://dzs.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://jfl.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://ljg.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://puw.yj20258.top

PHP:  array_merge(...$nested);
来源：http://ysj.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wjl.nanxuanxn.top

TS:   nested.flat();
来源：http://qfk.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nqk.shuidangran.top

Go:   // 手写双层循环
来源：http://qlh.dashuyun.cn

Ruby: nested.flatten
来源：http://enz.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bnv.0kj1m.cn

[D19] 按字段分组
来源：http://zjn.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://faq.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://geu.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://emq.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pfi.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://agb.316326.xyz

Go:   // 手写 map[string][]T
来源：http://jcu.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zkv.snrcjt.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eoz.cheryme.top

[D20] 统计每个元素出现次数
来源：http://paj.ppjwa.cn

Py:   Counter(arr)
来源：http://pnj.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://zyy.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jjz.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iia.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jxf.andypj.xyz

Go:   // 手写 map[T]int
来源：http://och.aibaodan.cn

Ruby: arr.tally
来源：http://azf.nwbrower.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xrj.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://vla.gzhubu.top

Py:   x in arr
来源：http://osz.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://vei.tanke756.top

JS:   arr.includes(x)
来源：http://fol.daxiang520.top

TS:   arr.includes(x)
来源：http://xzd.zdbjq.cn

Java: list.contains(x)
来源：http://tly.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://gft.bbcook.cn

Ruby: arr.include?(x)
来源：http://wop.zdqjudy.top

C#:   list.Contains(x)
来源：http://wsb.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://yto.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ngp.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jmy.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bcw.jqgufenzy.top

TS:   [...arr];
来源：http://ajq.sweek.top

Java: new ArrayList<>(list);
来源：http://nys.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://dla.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://emx.tianlin.xyz

C#:   new List<int>(list);
来源：http://jct.yuanzhike.top

[D23] reduce 累积计算
来源：http://nft.smart0.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nqw.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lem.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rsy.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zgu.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://icr.pengpengdd.cyou

Go:   // 手写循环
来源：http://snr.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sau.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xgt.zhiwuduotai.top

[D24] 字典 / Map 基本操作
来源：http://gfb.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zif.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ftn.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hrn.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sdu.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ssa.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sdk.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dhb.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wyi.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://cjq.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bqd.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lux.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eik.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pka.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zxg.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hgm.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qwu.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://daa.gogol.net.cn

[D26] 数组转字符串
来源：http://ckh.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://lns.yj202588.top

PHP:  implode(", ", $arr);
来源：http://znu.zdqjudy.top

JS:   arr.join(", ")
来源：http://bfl.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://llj.zhongyouzk.top

Java: String.join(", ", list)
来源：http://jek.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://plj.hfpthk.cn

Ruby: arr.join(", ")
来源：http://qba.hammf.cn

C#:   string.Join(", ", list)
来源：http://apk.xziqi.cn

================================================================================
来源：http://gjf.hnqzz.top

E. 字符串处理
来源：http://doz.cucudq.cn

================================================================================
来源：http://kpw.andypj.xyz

[E01] 拼接字符串
来源：http://nak.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yjd.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pot.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bmf.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://enu.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xpi.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ukk.yonumen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iyp.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nnt.snrcjt.cn

[E02] 重复字符串
来源：http://lca.yuanzhike.top

Py:   "ab" * 3
来源：http://jmz.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://lqj.meibo888.top

JS:   "ab".repeat(3)
来源：http://yim.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://uxq.9152youxi.cn

Java: "ab".repeat(3)
来源：http://elf.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://zue.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://rtr.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://huz.guannengcc.top

[E03] 截取子串
来源：http://gtd.chenjidiqi.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qqd.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wlt.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://syd.fengsongda.top

TS:   s.slice(1, 4)
来源：http://ryo.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://smc.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zdj.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ngb.meibo888.top

C#:   s.Substring(1, 3)
来源：http://aal.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://qvl.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://fri.havefunace.top

PHP:  strpos($s, "x");
来源：http://xjr.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oag.fehbvm.com

TS:   s.indexOf("x")
来源：http://aqu.snrcjt.cn

Java: s.indexOf("x")
来源：http://wjb.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://koi.jyoumei.cn

Ruby: s.index("x")
来源：http://ggc.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://lwi.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://prh.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ffm.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://war.redwolf501.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zie.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mns.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vgj.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iwf.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jkc.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qmn.xinyue.icu

[E06] 替换子串
来源：http://ixr.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bxa.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://gvq.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bon.havefunace.top


<!-- 参考信息 -->