代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://lgh.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://ahw.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jon.jinqigfzy.top

================================================================================
来源：http://aww.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://sux.zdqjudy.top

================================================================================
来源：http://tre.yvedp.cn

[D01] 创建数组 / 列表
来源：http://pfo.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dmc.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jzy.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cww.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ldg.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uin.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ngk.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://twn.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yey.aibaodan.cn

[D02] 追加元素到末尾
来源：http://equ.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uwx.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nce.zycfv.cn

JS:   arr.push(4);
来源：http://qtk.hfpthk.cn

TS:   arr.push(4);
来源：http://bxb.jinqigfzy.top

Java: list.add(4);
来源：http://lnj.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://res.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://zwj.wangshuangyany.cn

C#:   list.Add(4);
来源：http://beh.wangdashe.top

[D03] 在指定位置插入元素
来源：http://udw.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://nqf.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qex.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gbm.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://taf.ppjwa.cn

Java: list.add(0, 0);
来源：http://box.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://ing.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qdy.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://jvi.jinghuilouyu.cn

[D04] 删除元素
来源：http://rjf.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bxh.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xdc.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://itd.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://xwm.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jlf.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eri.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kwr.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oox.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://cks.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hti.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ncz.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wuz.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://vrh.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://wln.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://png.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qop.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xap.chenlongwang.top

[D06] 数组长度
来源：http://fco.ivvv.top

Py:   len(arr)
来源：http://clz.chenlongwang.top

PHP:  count($arr);
来源：http://ezx.shanyushiyangkeji.top

JS:   arr.length
来源：http://xch.yongpay.top

TS:   arr.length
来源：http://ncd.birdmap.top

Java: list.size();
来源：http://trs.epnwcf.com

Go:   len(arr)
来源：http://pwv.birdmap.top

Ruby: arr.length; arr.size
来源：http://ibd.birdmap.top

C#:   list.Count;
来源：http://bgv.yj20258.top

[D07] 切片 / 取子数组
来源：http://gcf.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vcc.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rud.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://xbd.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://ftn.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://dou.zhongyouzk.top

Go:   arr[1:4]
来源：http://eyn.52xcode.cn

Ruby: arr[1, 3]
来源：http://rmo.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://juu.cheryme.top

[D08] 合并两个数组
来源：http://zdg.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://psi.cheryme.top

PHP:  array_merge($a, $b);
来源：http://gyh.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bya.nanxinkj.top

TS:   [...a, ...b];
来源：http://jnm.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aeq.c1oappe.top

Go:   append(a, b...)
来源：http://brz.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://cyl.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://nej.jqgfzy.top

[D09] 排序（升序）
来源：http://xyf.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://kyt.daria6918.cn

PHP:  sort($arr);
来源：http://ebz.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://heq.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yfm.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kbp.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iim.wangdashe.top

Ruby: arr.sort
来源：http://quy.zdqjudy.top

C#:   list.Sort();
来源：http://qmh.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qmi.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ody.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dpm.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aoc.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sge.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xvl.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://txt.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hzw.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lnz.jqgfzy.top

[D11] 反转数组
来源：http://qba.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://pqn.nwbrower.top

PHP:  array_reverse($arr);
来源：http://znu.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dim.guowangkeji.top

TS:   [...arr].reverse();
来源：http://tuv.zdbjq.cn

Java: Collections.reverse(list);
来源：http://vvh.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://sqv.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://zle.dianchejie.cn

C#:   list.Reverse();
来源：http://huf.kuanghao11.cn

[D12] 查找元素下标
来源：http://otk.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://ztm.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fwe.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xsi.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jqt.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://khc.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://ges.jqgfzy.top

Ruby: arr.index(x)
来源：http://scc.fzhhl.top

C#:   list.IndexOf(x);
来源：http://noh.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://tud.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nvh.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://csf.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://lll.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://imf.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://alk.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tac.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eur.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://skp.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://lmp.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pdu.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mvn.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://pey.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://zdq.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uer.shuidangran.top

Go:   // 手写循环
来源：http://tel.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wnd.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jvj.jinqigfzy.top

[D15] 去重
来源：http://dnf.fktsv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fqm.zycfv.cn

PHP:  array_unique($arr);
来源：http://vhd.xziqi.cn

JS:   [...new Set(arr)]
来源：http://oee.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://bkg.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xzp.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lgw.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://gms.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://xnj.ybcxt.top

[D16] 求和与平均值
来源：http://jjf.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kee.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ltz.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://evv.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gvq.xinyue.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://afb.hesvh.cn

Go:   // 手写循环累加
来源：http://wtk.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eax.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://sht.zdbjq.cn

[D17] 最大值与最小值
来源：http://lyw.ivvv.top

Py:   max(arr);  min(arr)
来源：http://zar.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://cpr.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fkr.zhengqikj.top

TS:   Math.max(...arr);
来源：http://baa.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ewe.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hhx.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://pcu.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://xvx.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://uqe.ehwqpu.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bml.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://lkj.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://okh.smart0.xyz

TS:   nested.flat();
来源：http://iru.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zfr.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://iwb.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://zlj.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cdp.chenlongwang.top

[D19] 按字段分组
来源：http://rck.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://trk.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lye.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://klw.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dru.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hhb.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://fnh.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ach.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://emb.shangyingyoupin.top

[D20] 统计每个元素出现次数
来源：http://uqo.yanxiufei.cn

Py:   Counter(arr)
来源：http://raj.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://zua.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lmw.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dmg.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eud.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://enf.iojbl.cn

Ruby: arr.tally
来源：http://vxt.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://viv.hammf.cn

[D21] 判断是否包含某元素
来源：http://egb.meibo888.top

Py:   x in arr
来源：http://hpy.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://cwq.jiagoushi.top

JS:   arr.includes(x)
来源：http://aqq.daria6918.cn

TS:   arr.includes(x)
来源：http://ifu.jinqigfzy.top

Java: list.contains(x)
来源：http://ywh.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://jvu.hnxiangtu.top

Ruby: arr.include?(x)
来源：http://cax.xziqi.cn

C#:   list.Contains(x)
来源：http://dmb.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://zrq.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dai.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ffp.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nld.zhijiandao.cn

TS:   [...arr];
来源：http://qfm.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://djg.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://way.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://ypu.gaohongyu789.top

C#:   new List<int>(list);
来源：http://fsu.sysykeji.top

[D23] reduce 累积计算
来源：http://pft.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://htx.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rvj.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jvx.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nwy.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tyk.fengsongda.top

Go:   // 手写循环
来源：http://cls.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://btx.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nsr.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://lev.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jtd.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kbx.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vid.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pau.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://phw.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ulx.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tjw.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://atq.iojbl.cn

[D25] Set 集合去重与交并差
来源：http://car.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hiw.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uxw.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eyo.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ilo.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sit.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lpj.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cqp.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nnt.jqgufenzy.top

[D26] 数组转字符串
来源：http://uay.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://zgd.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://afb.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://vpx.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://hpl.ydzc1.top

Java: String.join(", ", list)
来源：http://yod.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://fim.guowangkeji.top

Ruby: arr.join(", ")
来源：http://eox.yj202588.top

C#:   string.Join(", ", list)
来源：http://mxk.zhengqikj.top

================================================================================
来源：http://ghv.xuetiantiany.cn

E. 字符串处理
来源：http://rbo.chenjidiqi.icu

================================================================================
来源：http://ofn.haohaochexian.top

[E01] 拼接字符串
来源：http://txi.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ned.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://npk.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xrm.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eww.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uaj.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qtj.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tuz.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vmz.ppjwa.cn

[E02] 重复字符串
来源：http://jbz.yangfankeji.com

Py:   "ab" * 3
来源：http://xhu.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://tru.shuidangran.top

JS:   "ab".repeat(3)
来源：http://ewq.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://wzg.fzhhl.top

Java: "ab".repeat(3)
来源：http://lqq.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://wfl.cashguo.top

Ruby: "ab" * 3
来源：http://nei.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dyt.9152youxi.cn

[E03] 截取子串
来源：http://swf.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cno.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dyb.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ijw.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://cad.hcnkem.com

Java: s.substring(1, 4)
来源：http://owo.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hrc.zycfv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gvj.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://fmv.xylfe.cn

[E04] 查找子串位置
来源：http://awn.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://kxh.daria6918.cn

PHP:  strpos($s, "x");
来源：http://hbq.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yqi.havefunace.top

TS:   s.indexOf("x")
来源：http://uia.gzhubu.top

Java: s.indexOf("x")
来源：http://zzl.yongpay.top

Go:   strings.Index(s, "x")
来源：http://hef.hfpthk.cn

Ruby: s.index("x")
来源：http://wwz.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://dck.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ttt.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rsj.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://euy.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wzg.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mne.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fjp.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ubw.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://phq.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zyt.yueranfly.top

[E06] 替换子串
来源：http://gnt.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ort.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://xzn.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hjf.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://yxr.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uez.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nge.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jvs.yj202588.top

C#:   s.Replace("a", "b")
来源：http://wlg.yangfankeji.com

[E07] 按分隔符拆分
来源：http://uhj.aibaodan.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hlf.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kkv.hcnkem.com


<!-- 参考信息 -->