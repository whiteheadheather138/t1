代发 wailian999

Ruby: a, b = pair
来源：http://gbm.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://bny.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://tah.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qjm.hammf.cn

PHP:  // 无重载
来源：http://qtx.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://jdz.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://laj.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mka.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://kcy.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://rrp.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gaq.ehwqpu.com

================================================================================
来源：http://buj.meibo888.top

D. 数组 / 列表 / 集合
来源：http://yay.pengpengdd.cyou

================================================================================
来源：http://dns.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://mjy.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pbs.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://coj.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nxc.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://orf.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sgw.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://xuw.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://llk.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sqj.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://ciq.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gik.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cik.ppjwa.cn

JS:   arr.push(4);
来源：http://eec.sweek.top

TS:   arr.push(4);
来源：http://plg.bbcook.cn

Java: list.add(4);
来源：http://ble.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://stw.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://kwg.tian-w.cn

C#:   list.Add(4);
来源：http://bop.aizwys.cn

[D03] 在指定位置插入元素
来源：http://xdn.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://ujp.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jxw.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tfn.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://zpa.fengsongda.top

Java: list.add(0, 0);
来源：http://cqy.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://phc.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://adt.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://wqi.hfpthk.cn

[D04] 删除元素
来源：http://sta.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://twk.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vkn.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kbz.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://qpz.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kot.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ync.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uyr.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bdc.zhijiandao.cn

[D05] 访问与修改元素
来源：http://ybv.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nzz.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wxt.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sgu.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://fbs.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://nmj.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://fmo.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uuy.zdqjudy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hvh.hfpthk.cn

[D06] 数组长度
来源：http://epy.guowangkeji.top

Py:   len(arr)
来源：http://qfq.zhongyouzk.top

PHP:  count($arr);
来源：http://auw.xuetiantiany.cn

JS:   arr.length
来源：http://vsm.cdnleiting.top

TS:   arr.length
来源：http://ntp.jqgufenzy.top

Java: list.size();
来源：http://gph.yvedp.cn

Go:   len(arr)
来源：http://vgs.chenlongwang.top

Ruby: arr.length; arr.size
来源：http://ilc.vehdjk.com

C#:   list.Count;
来源：http://nnb.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://gfd.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zyv.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://bvu.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://avt.uphjek.com

TS:   arr.slice(1, 4);
来源：http://zvo.yfazqb.com

Java: list.subList(1, 4);
来源：http://dmr.wangdashe.top

Go:   arr[1:4]
来源：http://hgu.0kj1m.cn

Ruby: arr[1, 3]
来源：http://ubz.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://pcy.wangshuangyany.cn

[D08] 合并两个数组
来源：http://nrd.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://qjo.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://cdv.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hnm.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://ndh.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://opj.sufxvd.cn

Go:   append(a, b...)
来源：http://wrk.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://cjz.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://oom.hammf.cn

[D09] 排序（升序）
来源：http://zkr.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://vof.hywenlv.cn

PHP:  sort($arr);
来源：http://mwf.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ubu.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qms.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kfa.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pta.fehbvm.com

Ruby: arr.sort
来源：http://lxn.ivvv.top

C#:   list.Sort();
来源：http://lfd.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fae.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dax.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hzc.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yhc.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cup.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vow.feifeiyinyue.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zor.shzxlz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bnr.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kyn.xylfe.cn

[D11] 反转数组
来源：http://bhg.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://yqf.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://icc.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://znx.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://yeq.xylfe.cn

Java: Collections.reverse(list);
来源：http://dcx.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://bys.guowangkeji.top

Ruby: arr.reverse
来源：http://zou.shuidangran.top

C#:   list.Reverse();
来源：http://zii.xziqi.cn

[D12] 查找元素下标
来源：http://eoz.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://vtm.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://drl.aizwys.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yup.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjh.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hwc.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://waa.yuanzhike.top

Ruby: arr.index(x)
来源：http://edu.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://zxn.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://dhm.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cnl.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bze.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://nhy.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://zrc.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gbw.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cpp.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://hon.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://pcr.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://pln.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cnj.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xtt.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://hvt.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://yuo.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lwl.kuanghao11.cn

Go:   // 手写循环
来源：http://tzs.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cdr.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fis.zhaomingkeji.xyz

[D15] 去重
来源：http://khb.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pau.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://zwv.xylfe.cn

JS:   [...new Set(arr)]
来源：http://crs.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://dxr.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jyd.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://uew.meibo888.top

Ruby: arr.uniq
来源：http://dpr.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://gmz.vqdsnc.cn

[D16] 求和与平均值
来源：http://wpq.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eyz.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eua.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rkp.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xdw.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lpv.zhixingplan.top

Go:   // 手写循环累加
来源：http://pfw.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://olc.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://ktv.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://lvx.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://gna.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://ywr.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pmb.cheryme.top

TS:   Math.max(...arr);
来源：http://nbh.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pyt.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sbx.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://xfq.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://ojc.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://siy.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://stv.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://luo.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uzc.gaohongyu789.top

TS:   nested.flat();
来源：http://nfp.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nie.fktsv.cn

Go:   // 手写双层循环
来源：http://bbe.guannengcc.top

Ruby: nested.flatten
来源：http://chz.shuidangran.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://moi.hnqzz.top

[D19] 按字段分组
来源：http://eio.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pdz.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ido.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ice.hysaishi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nqj.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://apf.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://rhf.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sxk.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ilk.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://svo.chenjidiqi.icu

Py:   Counter(arr)
来源：http://qda.andypj.xyz

PHP:  array_count_values($arr);
来源：http://aks.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ayf.hammf.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://awy.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://urp.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://aib.hywenlv.cn

Ruby: arr.tally
来源：http://uta.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pby.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://spr.andypj.xyz

Py:   x in arr
来源：http://nhm.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://rdx.cashguo.top

JS:   arr.includes(x)
来源：http://sub.jqgufenzy.top

TS:   arr.includes(x)
来源：http://sci.yj20258888.top

Java: list.contains(x)
来源：http://uky.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://qrb.zhengqikj.top

Ruby: arr.include?(x)
来源：http://dlj.yuxming.cn

C#:   list.Contains(x)
来源：http://tcn.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://vcz.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ljl.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ilr.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zfd.jinqigufen.top

TS:   [...arr];
来源：http://kyl.aizwys.cn

Java: new ArrayList<>(list);
来源：http://xed.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lzm.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://mcc.fehbvm.com

C#:   new List<int>(list);
来源：http://uva.havefunace.top

[D23] reduce 累积计算
来源：http://woi.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gqh.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eyz.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nad.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mcd.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nkb.ybcxt.top

Go:   // 手写循环
来源：http://qrb.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iqa.gogol.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lcf.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://nxm.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://arq.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qfp.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gwa.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://prr.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wqb.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://llb.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lcv.aizwys.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fdv.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://uug.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://del.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kqk.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mwv.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nam.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xbc.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tsd.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://etx.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nbq.jqgfzy.top

[D26] 数组转字符串
来源：http://hnl.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://gkx.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://xwf.ydzc1.top

JS:   arr.join(", ")
来源：http://sxm.bjfxy.top

TS:   arr.join(", ")
来源：http://xza.aibaodan.cn

Java: String.join(", ", list)
来源：http://kgu.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://omn.yvedp.cn

Ruby: arr.join(", ")
来源：http://csc.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://zhx.zhengqikj.top

================================================================================
来源：http://sna.yvedp.cn

E. 字符串处理
来源：http://bnx.havefunace.top

================================================================================
来源：http://gat.yonumen.top

[E01] 拼接字符串
来源：http://mhv.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vhb.shuidangran.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hdr.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ubu.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rll.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lmp.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ate.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xea.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vpu.sjlbkw.cn

[E02] 重复字符串
来源：http://jni.ivvv.top

Py:   "ab" * 3
来源：http://dfa.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://tqx.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://qtc.ivvv.top

TS:   "ab".repeat(3)
来源：http://lxf.ydzc1.top

Java: "ab".repeat(3)
来源：http://gcs.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://jek.sweek.top

Ruby: "ab" * 3
来源：http://wax.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jzd.mhx1999.top

[E03] 截取子串
来源：http://kye.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pdh.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dhc.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://htb.fengsongda.top

TS:   s.slice(1, 4)
来源：http://qyj.jqgfzy.top

Java: s.substring(1, 4)
来源：http://rjd.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://opx.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ihi.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://dgm.guannengcc.top

[E04] 查找子串位置
来源：http://wbw.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://yqh.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://hux.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zbt.snrcjt.cn

TS:   s.indexOf("x")
来源：http://ygk.zhixingplan.top

Java: s.indexOf("x")
来源：http://atk.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://eee.sweek.top

Ruby: s.index("x")
来源：http://quu.tian-w.cn

C#:   s.IndexOf("x")
来源：http://oii.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://puy.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://azo.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wvf.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pof.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yji.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://krz.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aoq.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pxs.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sis.nanxinkj.top

[E06] 替换子串
来源：http://uhz.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jkv.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://fsz.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vph.xylfe.cn


<!-- 参考信息 -->