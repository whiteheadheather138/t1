代发 wailian999

Ruby: a, b = pair
来源：http://edj.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://ehk.hfpthk.cn

[C16] 函数 / 方法重载
来源：http://eco.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uoh.birdmap.top

PHP:  // 无重载
来源：http://hum.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ema.0kj1m.cn

TS:   // 用联合类型或重载签名声明
来源：http://ewj.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qok.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://qdu.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://cim.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://abz.9152youxi.cn

================================================================================
来源：http://thu.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://ahu.xuanzx.com

================================================================================
来源：http://xoo.yj20258888.top

[D01] 创建数组 / 列表
来源：http://tay.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vhg.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ylg.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://olc.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fbt.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uor.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://fbn.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://rdf.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mmy.fengsongda.top

[D02] 追加元素到末尾
来源：http://qtw.ctjpmb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://trx.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sqv.hammf.cn

JS:   arr.push(4);
来源：http://job.yonumen.top

TS:   arr.push(4);
来源：http://qej.yueranfly.top

Java: list.add(4);
来源：http://ofp.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://khe.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://oax.tarul.cn

C#:   list.Add(4);
来源：http://wyc.andypj.xyz

[D03] 在指定位置插入元素
来源：http://usr.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://dxa.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fws.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vmj.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://nkb.jiagoushi.top

Java: list.add(0, 0);
来源：http://xxx.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://htg.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kqv.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://bwm.shangyingyoupin.top

[D04] 删除元素
来源：http://vto.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cer.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iil.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ees.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://swi.shzxlz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sbh.hnqzz.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yfp.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://enx.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jhz.yongpay.top

[D05] 访问与修改元素
来源：http://elu.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xqq.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zkh.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://auv.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://fbh.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://zhd.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://mpe.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fwr.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cmz.xuetiantiany.cn

[D06] 数组长度
来源：http://hci.guowangkeji.top

Py:   len(arr)
来源：http://cdy.yueranfly.top

PHP:  count($arr);
来源：http://qsy.ydjk.org.cn

JS:   arr.length
来源：http://xqf.feifeiyinyue.top

TS:   arr.length
来源：http://srt.meibo888.top

Java: list.size();
来源：http://wwx.ctjpmb.com

Go:   len(arr)
来源：http://yfa.ppjwa.cn

Ruby: arr.length; arr.size
来源：http://djo.iojbl.cn

C#:   list.Count;
来源：http://cvl.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://vsg.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://riu.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://snn.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://vgp.nwbrower.top

TS:   arr.slice(1, 4);
来源：http://tvk.daria6918.cn

Java: list.subList(1, 4);
来源：http://zmq.c1oappe.top

Go:   arr[1:4]
来源：http://qoe.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://exx.epnwcf.com

C#:   list.GetRange(1, 3);
来源：http://kel.xuanzx.com

[D08] 合并两个数组
来源：http://ehe.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://uwa.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://doc.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iiv.epnwcf.com

TS:   [...a, ...b];
来源：http://olb.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rpq.tianlin.xyz

Go:   append(a, b...)
来源：http://zyb.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://trh.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://vwl.cdnleiting.top

[D09] 排序（升序）
来源：http://mrn.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://pzx.zhongyouzk.top

PHP:  sort($arr);
来源：http://qhp.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fcx.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://hro.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://fpg.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://frg.fanxiaobao.xyz

Ruby: arr.sort
来源：http://efq.hammf.cn

C#:   list.Sort();
来源：http://dix.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mcy.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://swv.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kjy.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dvc.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cmi.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mnu.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lcf.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lwd.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ral.tarul.cn

[D11] 反转数组
来源：http://mms.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://lyb.52xcode.cn

PHP:  array_reverse($arr);
来源：http://egm.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ozd.sysykeji.top

TS:   [...arr].reverse();
来源：http://mxi.smart0.xyz

Java: Collections.reverse(list);
来源：http://eam.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://hyb.zhongyouzk.top

Ruby: arr.reverse
来源：http://tcr.meibo888.top

C#:   list.Reverse();
来源：http://ymt.redwolf501.top

[D12] 查找元素下标
来源：http://vai.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://yjo.hnxiangtu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tke.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cii.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dgl.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://agk.guowangkeji.top

Go:   slices.Index(arr, x)
来源：http://yql.ydzc1.top

Ruby: arr.index(x)
来源：http://epr.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://iyt.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://toq.zdbjq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hic.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bet.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://nbs.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://plo.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hbp.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fxd.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://icg.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mgx.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://eew.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rxw.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ukz.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://pba.shzxlz.cn

TS:   arr.map(x => x * 2)
来源：http://zwe.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://dif.cucudq.cn

Go:   // 手写循环
来源：http://mfl.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://dxh.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hdq.havefunace.top

[D15] 去重
来源：http://mpo.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ykv.jyoumei.cn

PHP:  array_unique($arr);
来源：http://lzt.havefunace.top

JS:   [...new Set(arr)]
来源：http://umh.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://qgg.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xte.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://sef.hongshengwenyu.top

Ruby: arr.uniq
来源：http://vjl.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://rfh.chenlongwang.top

[D16] 求和与平均值
来源：http://zls.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sdg.bjfxy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qri.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sws.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oyf.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cyl.havefunace.top

Go:   // 手写循环累加
来源：http://umm.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qhk.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://abf.haohaochexian.top

[D17] 最大值与最小值
来源：http://vyt.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://oxb.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://oou.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rnq.dianchejie.cn

TS:   Math.max(...arr);
来源：http://moc.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hvk.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nod.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://oon.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://dtr.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://ofk.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kez.birdmap.top

PHP:  array_merge(...$nested);
来源：http://kju.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mgy.ehwqpu.com

TS:   nested.flat();
来源：http://rct.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://azk.dashuyun.cn

Go:   // 手写双层循环
来源：http://ckf.nanxinkj.top

Ruby: nested.flatten
来源：http://sto.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kpv.guowangkeji.top

[D19] 按字段分组
来源：http://wwf.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xqf.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dry.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kuu.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hys.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jho.yongpay.top

Go:   // 手写 map[string][]T
来源：http://xgt.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://bbu.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rxt.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://wtg.guowangkeji.top

Py:   Counter(arr)
来源：http://dli.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://zzu.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jnr.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fkc.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yxr.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://xkw.tianlin.xyz

Ruby: arr.tally
来源：http://dqg.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pke.birdmap.top

[D21] 判断是否包含某元素
来源：http://ccw.tianlin.xyz

Py:   x in arr
来源：http://zga.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://xil.jinqigufen.top

JS:   arr.includes(x)
来源：http://pja.svipenyu.cn

TS:   arr.includes(x)
来源：http://qso.feifeiyinyue.top

Java: list.contains(x)
来源：http://kcs.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://wof.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://eyx.yongpay.top

C#:   list.Contains(x)
来源：http://kwv.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://rci.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rht.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://enn.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aum.sweek.top

TS:   [...arr];
来源：http://aqb.yvedp.cn

Java: new ArrayList<>(list);
来源：http://vke.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xpm.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://svi.yfazqb.com

C#:   new List<int>(list);
来源：http://yol.ppjwa.cn

[D23] reduce 累积计算
来源：http://gqi.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lht.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xhf.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vfd.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fjl.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://zvz.guowangkeji.top

Go:   // 手写循环
来源：http://ykr.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://icf.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qga.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://kxd.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fyq.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wrr.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ylp.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hhy.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ccn.guowangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rng.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hna.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nei.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://jyw.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dgo.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zqb.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://asz.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dey.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jcf.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yec.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://efz.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ola.sweek.top

[D26] 数组转字符串
来源：http://ute.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://lzi.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://hbf.meibo888.top

JS:   arr.join(", ")
来源：http://tkg.shzxlz.cn

TS:   arr.join(", ")
来源：http://kdu.tanke756.top

Java: String.join(", ", list)
来源：http://xsm.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://xsw.gzhubu.top

Ruby: arr.join(", ")
来源：http://fjv.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://uny.wangdashe.top

================================================================================
来源：http://wtz.sufxvd.cn

E. 字符串处理
来源：http://qeg.zhaomingkeji.xyz

================================================================================
来源：http://gqp.316326.xyz

[E01] 拼接字符串
来源：http://rhf.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gzd.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ieh.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hnv.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rfe.jinyuanbaomall.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xfs.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qcs.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hhs.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://loh.nanxinkj.top

[E02] 重复字符串
来源：http://dff.zdqjudy.top

Py:   "ab" * 3
来源：http://gzu.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://jey.hongshengwenyu.top

JS:   "ab".repeat(3)
来源：http://kmn.dashuyun.cn

TS:   "ab".repeat(3)
来源：http://ocf.ppjwa.cn

Java: "ab".repeat(3)
来源：http://kzo.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://eik.shuidangran.top

Ruby: "ab" * 3
来源：http://zps.guowangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jye.ybcxt.top

[E03] 截取子串
来源：http://mbf.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xxk.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://duu.shangyingyoupin.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dso.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://ayc.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://tqb.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jpx.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://xps.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://bdj.yueranfly.top

[E04] 查找子串位置
来源：http://ymf.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://yzn.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://elh.smart0.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uag.hnqzz.top

TS:   s.indexOf("x")
来源：http://flu.nanxinkj.top

Java: s.indexOf("x")
来源：http://urm.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://dio.yongpay.top

Ruby: s.index("x")
来源：http://gcn.yueranfly.top

C#:   s.IndexOf("x")
来源：http://nxy.hywenlv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mwz.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zxk.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bcl.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nng.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eeu.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://efu.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://adw.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://igc.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jab.ctjpmb.com

[E06] 替换子串
来源：http://jho.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fqm.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://txq.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bgs.redwolf501.top


<!-- 参考信息 -->