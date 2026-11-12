代发 wailian999

Ruby: a, b = pair
来源：http://bqn.316326.xyz

C#:   var (a, b) = pair;
来源：http://alq.yuxming.cn

[C16] 函数 / 方法重载
来源：http://zvz.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ahb.wangdashe.top

PHP:  // 无重载
来源：http://uke.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://msp.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://tbf.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yfj.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://xqt.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://phy.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://agh.svipenyu.cn

================================================================================
来源：http://eax.uphjek.com

D. 数组 / 列表 / 集合
来源：http://itv.sweek.top

================================================================================
来源：http://emg.birdmap.top

[D01] 创建数组 / 列表
来源：http://icz.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xyg.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vku.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qzc.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://psq.yueranfly.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://muy.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://mbb.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://dlw.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hnb.cdnleiting.top

[D02] 追加元素到末尾
来源：http://tbg.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hem.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mon.yfazqb.com

JS:   arr.push(4);
来源：http://icf.zhengqikj.top

TS:   arr.push(4);
来源：http://jst.haohaochexian.top

Java: list.add(4);
来源：http://gxr.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://wpc.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://ohl.yangfankeji.com

C#:   list.Add(4);
来源：http://gim.yj202588.top

[D03] 在指定位置插入元素
来源：http://vcl.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://gld.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xhd.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hcf.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://zlf.hywenlv.cn

Java: list.add(0, 0);
来源：http://jme.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://xmr.xziqi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wgh.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://vkm.sxryk.cn

[D04] 删除元素
来源：http://qyc.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nef.cqqwz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zbs.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://srz.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://wdr.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qqr.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zbs.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kni.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lxh.yangfankeji.com

[D05] 访问与修改元素
来源：http://eos.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lpk.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://prl.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dsj.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://gnb.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://qnn.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://ngq.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kfi.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eau.guannengcc.top

[D06] 数组长度
来源：http://qms.tarul.cn

Py:   len(arr)
来源：http://pgj.wangshuangyany.cn

PHP:  count($arr);
来源：http://tyh.vehdjk.com

JS:   arr.length
来源：http://feq.yuxming.cn

TS:   arr.length
来源：http://tkl.ydzc1.top

Java: list.size();
来源：http://aaw.sweek.top

Go:   len(arr)
来源：http://ovn.c1oappe.top

Ruby: arr.length; arr.size
来源：http://gml.yj20258.top

C#:   list.Count;
来源：http://apl.sxryk.cn

[D07] 切片 / 取子数组
来源：http://kvs.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wld.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://wnm.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://cgt.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://snr.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://tcz.xylfe.cn

Go:   arr[1:4]
来源：http://sem.iojbl.cn

Ruby: arr[1, 3]
来源：http://zyb.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://wuk.wangshuangyany.cn

[D08] 合并两个数组
来源：http://bal.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://zqe.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://cyg.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xss.tarul.cn

TS:   [...a, ...b];
来源：http://mno.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dsl.jianghu66.top

Go:   append(a, b...)
来源：http://fld.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://slr.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://uoa.sysykeji.top

[D09] 排序（升序）
来源：http://knp.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://aqk.c1oappe.top

PHP:  sort($arr);
来源：http://lgl.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dvt.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vza.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nrd.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zot.kuanghao11.cn

Ruby: arr.sort
来源：http://jtz.tarul.cn

C#:   list.Sort();
来源：http://lwf.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vuc.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cnk.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bcl.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qmo.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zzj.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ooq.snrcjt.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wyp.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uxv.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://heu.xinyue.icu

[D11] 反转数组
来源：http://iap.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://ynr.chenlongwang.top

PHP:  array_reverse($arr);
来源：http://dbk.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vhk.fzhhl.top

TS:   [...arr].reverse();
来源：http://tlf.cheryme.top

Java: Collections.reverse(list);
来源：http://crb.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://wxb.ydzc1.top

Ruby: arr.reverse
来源：http://knu.hfpthk.cn

C#:   list.Reverse();
来源：http://zwl.xuetiantiany.cn

[D12] 查找元素下标
来源：http://xze.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://krt.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wfd.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vpe.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://njj.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://knk.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://pdc.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://ozv.cashguo.top

C#:   list.IndexOf(x);
来源：http://voq.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://doe.tanke756.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bqq.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rjr.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://yup.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://spu.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tfl.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xco.zhiwuduotai.top

Ruby: arr.select { |x| x > 3 }
来源：http://gbs.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ovw.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://qny.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rhc.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fyt.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://jyx.sweek.top

TS:   arr.map(x => x * 2)
来源：http://pzh.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://utb.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://pum.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://vss.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://yex.fengsongda.top

[D15] 去重
来源：http://mwr.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xhy.yonumen.top

PHP:  array_unique($arr);
来源：http://gnp.sxryk.cn

JS:   [...new Set(arr)]
来源：http://jye.wangdashe.top

TS:   [...new Set(arr)]
来源：http://qlf.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gep.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://wic.vehdjk.com

Ruby: arr.uniq
来源：http://nus.zhongyouzk.top

C#:   list.Distinct().ToList()
来源：http://wuq.ctjpmb.com

[D16] 求和与平均值
来源：http://dtx.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qer.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hba.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aqc.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://srb.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://svy.yanxiufei.cn

Go:   // 手写循环累加
来源：http://ovz.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nxf.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://qdi.yj202588.top

[D17] 最大值与最小值
来源：http://pfn.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://avo.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://okt.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uhh.xinyue.icu

TS:   Math.max(...arr);
来源：http://ktr.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://qmv.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bva.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://nle.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://tsj.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://abx.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mra.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://pzd.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pbm.cucudq.cn

TS:   nested.flat();
来源：http://ajd.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://imf.sjlbkw.cn

Go:   // 手写双层循环
来源：http://vwc.daria6918.cn

Ruby: nested.flatten
来源：http://oew.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dse.cashguo.top

[D19] 按字段分组
来源：http://mgz.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xgj.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mvl.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dqo.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pdn.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qop.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://vaf.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tns.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rhh.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://oiu.jlsjyb.cn

Py:   Counter(arr)
来源：http://tdo.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://lve.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uqu.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oyb.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://knn.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://tsu.svipenyu.cn

Ruby: arr.tally
来源：http://cjy.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uak.52xcode.cn

[D21] 判断是否包含某元素
来源：http://euc.xylfe.cn

Py:   x in arr
来源：http://kch.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://isx.sjlbkw.cn

JS:   arr.includes(x)
来源：http://yop.vehdjk.com

TS:   arr.includes(x)
来源：http://ezd.redwolf501.top

Java: list.contains(x)
来源：http://gyg.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://bfd.yj202588.top

Ruby: arr.include?(x)
来源：http://xeq.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://wop.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://lyx.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gcz.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wwx.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cij.52xcode.cn

TS:   [...arr];
来源：http://wed.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://awl.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://tfu.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://hxy.vqdsnc.cn

C#:   new List<int>(list);
来源：http://jea.zhengqikj.top

[D23] reduce 累积计算
来源：http://tye.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://arj.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gzu.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://boc.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ald.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://lzv.guowangkeji.top

Go:   // 手写循环
来源：http://vjd.feifeiyinyue.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yjf.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cho.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://gjr.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oox.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gov.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://okn.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xrj.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://coi.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ufk.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vln.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hhj.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://gru.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zhg.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cus.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ruw.sxryk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gzu.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bhf.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mqx.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gih.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ptw.meibo888.top

[D26] 数组转字符串
来源：http://uzx.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://yqu.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://qwi.quarkkingdee.top

JS:   arr.join(", ")
来源：http://ulz.cheryme.top

TS:   arr.join(", ")
来源：http://sxy.yueranfly.top

Java: String.join(", ", list)
来源：http://yto.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://hdh.hfpthk.cn

Ruby: arr.join(", ")
来源：http://yco.shuidangran.top

C#:   string.Join(", ", list)
来源：http://dzz.jqgfzy.top

================================================================================
来源：http://alb.daria6918.cn

E. 字符串处理
来源：http://tzm.yangfankeji.com

================================================================================
来源：http://yay.xylfe.cn

[E01] 拼接字符串
来源：http://kup.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sbu.haohaochexian.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kbv.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ysw.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xwt.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dra.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bat.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bgi.shzxlz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nno.jinqigufen.top

[E02] 重复字符串
来源：http://kcc.cucudq.cn

Py:   "ab" * 3
来源：http://odi.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://aik.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://zhz.c1oappe.top

TS:   "ab".repeat(3)
来源：http://ile.snrcjt.cn

Java: "ab".repeat(3)
来源：http://wvf.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://uno.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://sfa.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ewc.nwbrower.top

[E03] 截取子串
来源：http://smy.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fkd.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sbd.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://osu.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://esz.yongpay.top

Java: s.substring(1, 4)
来源：http://djx.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ssa.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://pzg.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://exo.zhengqikj.top

[E04] 查找子串位置
来源：http://hoz.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://ijh.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://azp.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sts.hesvh.cn

TS:   s.indexOf("x")
来源：http://twi.tianlin.xyz

Java: s.indexOf("x")
来源：http://zwg.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://mij.hnxiangtu.top

Ruby: s.index("x")
来源：http://biw.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://apj.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wfi.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fic.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ffa.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://usf.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pxh.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mna.fzhhl.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://myl.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kmd.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mjo.zycfv.cn

[E06] 替换子串
来源：http://aym.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fxe.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://mcv.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sxu.ybcxt.top


<!-- 参考信息 -->