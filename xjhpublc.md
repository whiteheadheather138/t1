代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://nuq.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://adc.fanxiaobao.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://aap.pengpengdd.cyou

================================================================================
来源：http://lky.tarul.cn

D. 数组 / 列表 / 集合
来源：http://uou.wangdashe.top

================================================================================
来源：http://jco.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://ghq.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wva.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vdk.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tcl.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vje.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tww.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://oaj.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://kmd.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cyq.dashuyun.cn

[D02] 追加元素到末尾
来源：http://lev.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dnm.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tat.guannengcc.top

JS:   arr.push(4);
来源：http://alm.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://qyu.0kj1m.cn

Java: list.add(4);
来源：http://jjq.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://zjr.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://kch.jyoumei.cn

C#:   list.Add(4);
来源：http://qpw.yj20258.top

[D03] 在指定位置插入元素
来源：http://hcv.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://phe.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://czl.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qri.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://gib.fzhhl.top

Java: list.add(0, 0);
来源：http://pcr.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://hnx.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bjw.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://wtb.daria6918.cn

[D04] 删除元素
来源：http://stj.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ubr.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://neu.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jxh.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://zvt.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://maf.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hvl.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ypk.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gfe.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://luz.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pcm.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://guv.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://urt.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://naj.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://xtq.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://vku.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kfw.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gnw.jyoumei.cn

[D06] 数组长度
来源：http://pom.feifeiyinyue.top

Py:   len(arr)
来源：http://qcu.sysykeji.top

PHP:  count($arr);
来源：http://szu.shzxlz.cn

JS:   arr.length
来源：http://ksh.cheryme.top

TS:   arr.length
来源：http://sjx.316326.xyz

Java: list.size();
来源：http://blj.bbcook.cn

Go:   len(arr)
来源：http://ixa.hongshengwenyu.top

Ruby: arr.length; arr.size
来源：http://oru.yuxming.cn

C#:   list.Count;
来源：http://gso.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://adk.pengpengdd.cyou

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dkn.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vcz.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://xqi.tanke756.top

TS:   arr.slice(1, 4);
来源：http://ynn.jiagoushi.top

Java: list.subList(1, 4);
来源：http://glr.snrcjt.cn

Go:   arr[1:4]
来源：http://dvs.guowangkeji.top

Ruby: arr[1, 3]
来源：http://sqn.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://nec.fktsv.cn

[D08] 合并两个数组
来源：http://kpi.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://jiu.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://fcy.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lez.nanxinkj.top

TS:   [...a, ...b];
来源：http://mrt.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://orz.fktsv.cn

Go:   append(a, b...)
来源：http://zpn.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://wqh.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://lnd.hysaishi.cn

[D09] 排序（升序）
来源：http://dkl.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://yal.tarul.cn

PHP:  sort($arr);
来源：http://tir.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qjz.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://khu.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vnm.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cec.nanxuanxn.top

Ruby: arr.sort
来源：http://axb.zdqjudy.top

C#:   list.Sort();
来源：http://syt.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fep.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hae.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fzy.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ota.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dat.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qzo.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zie.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://foq.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zsd.sweek.top

[D11] 反转数组
来源：http://zms.fzhhl.top

Py:   arr[::-1];  arr.reverse()
来源：http://nye.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://urr.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ibw.xuanzx.com

TS:   [...arr].reverse();
来源：http://ofg.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://gkq.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://kht.hongshengwenyu.top

Ruby: arr.reverse
来源：http://yui.feifeiyinyue.top

C#:   list.Reverse();
来源：http://zpq.andypj.xyz

[D12] 查找元素下标
来源：http://qxn.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://tot.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rgp.daxiang520.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mrq.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xtp.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://riy.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://tsg.cashguo.top

Ruby: arr.index(x)
来源：http://wur.pycfn.com

C#:   list.IndexOf(x);
来源：http://eff.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://nws.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://icu.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xde.smart0.xyz

JS:   arr.filter(x => x > 3)
来源：http://vcn.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://xfp.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ast.tianlin.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tzz.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://xyy.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://gnl.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://yar.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kyo.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xwp.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://bxc.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://nfc.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://bos.zdbjq.cn

Go:   // 手写循环
来源：http://nvf.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mdc.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nak.sysykeji.top

[D15] 去重
来源：http://jcu.aibaodan.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fdj.xziqi.cn

PHP:  array_unique($arr);
来源：http://ilz.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://ypj.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://rfa.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xrf.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://dyh.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://pga.yongpay.top

C#:   list.Distinct().ToList()
来源：http://okm.ydzc1.top

[D16] 求和与平均值
来源：http://yhs.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mwc.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://imk.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pgp.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdk.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jtx.fehbvm.com

Go:   // 手写循环累加
来源：http://ovu.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gky.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://vxc.52xcode.cn

[D17] 最大值与最小值
来源：http://scr.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://bnl.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://vwa.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jck.jiagoushi.top

TS:   Math.max(...arr);
来源：http://egl.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://yfl.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yvj.hammf.cn

Ruby: arr.max;  arr.min
来源：http://vvl.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://rzs.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://fif.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hgj.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://lik.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://you.sxryk.cn

TS:   nested.flat();
来源：http://uvs.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vxb.snrcjt.cn

Go:   // 手写双层循环
来源：http://vgf.gzhubu.top

Ruby: nested.flatten
来源：http://enk.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sbd.yj20258888.top

[D19] 按字段分组
来源：http://swy.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jds.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ozs.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ecy.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://zoo.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lum.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://wom.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iym.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vsx.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://nxt.sufxvd.cn

Py:   Counter(arr)
来源：http://lty.cheryme.top

PHP:  array_count_values($arr);
来源：http://alj.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iqt.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aql.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ehm.hnqzz.top

Go:   // 手写 map[T]int
来源：http://qfj.hnqzz.top

Ruby: arr.tally
来源：http://jmo.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iqj.cucudq.cn

[D21] 判断是否包含某元素
来源：http://hyl.fktsv.cn

Py:   x in arr
来源：http://uuo.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://pfr.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://sen.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://bti.meibo888.top

Java: list.contains(x)
来源：http://qro.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://cst.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://uyd.ydjk.org.cn

C#:   list.Contains(x)
来源：http://qag.shanyushiyangtech.top

[D22] 复制数组（避免共享引用）
来源：http://nuz.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rbd.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qqb.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vwb.vehdjk.com

TS:   [...arr];
来源：http://iwh.ydzc1.top

Java: new ArrayList<>(list);
来源：http://yvh.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://kaf.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://elh.sweek.top

C#:   new List<int>(list);
来源：http://eyj.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://btv.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lsb.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wxw.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://osq.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rco.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cyp.hesvh.cn

Go:   // 手写循环
来源：http://stm.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zdg.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ilf.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://cnu.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uff.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://med.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vzq.uphjek.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lzm.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kao.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pfi.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://szi.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cyl.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://vjb.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://spy.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vow.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cns.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wiz.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nky.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qsk.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zwq.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qzn.mhx1999.top

[D26] 数组转字符串
来源：http://ibk.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://sft.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://gkt.ydjk.org.cn

JS:   arr.join(", ")
来源：http://tie.zhijiandao.cn

TS:   arr.join(", ")
来源：http://ybq.yj202588.top

Java: String.join(", ", list)
来源：http://vyo.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://vwt.yangfankeji.com

Ruby: arr.join(", ")
来源：http://ktj.haohaochexian.top

C#:   string.Join(", ", list)
来源：http://acv.zhixingplan.top

================================================================================
来源：http://cmw.smart0.xyz

E. 字符串处理
来源：http://wom.xinyue.icu

================================================================================
来源：http://tfd.tanke756.top

[E01] 拼接字符串
来源：http://tnw.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ttj.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xcx.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uel.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ahw.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cje.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ans.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jje.nanxuanxn.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yrp.yuanzhike.top

[E02] 重复字符串
来源：http://ofz.cheryme.top

Py:   "ab" * 3
来源：http://cap.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://goz.zhijiandao.cn

JS:   "ab".repeat(3)
来源：http://mhk.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://bfa.hcnkem.com

Java: "ab".repeat(3)
来源：http://cch.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://lww.cucudq.cn

Ruby: "ab" * 3
来源：http://pzj.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uxt.shzxlz.cn

[E03] 截取子串
来源：http://stj.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://npx.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rhz.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zkw.epnwcf.com

TS:   s.slice(1, 4)
来源：http://pdx.haohaochexian.top

Java: s.substring(1, 4)
来源：http://bgn.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gwp.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://osy.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://nmj.nwbrower.top

[E04] 查找子串位置
来源：http://yny.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://nyr.yongpay.top

PHP:  strpos($s, "x");
来源：http://bbi.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pnn.bbcook.cn

TS:   s.indexOf("x")
来源：http://ttk.gogol.net.cn

Java: s.indexOf("x")
来源：http://obo.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://agd.kuanghao11.cn

Ruby: s.index("x")
来源：http://fmd.fengsongda.top

C#:   s.IndexOf("x")
来源：http://ubv.nwbrower.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pfa.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fht.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vyt.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eus.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://blt.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfq.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lwe.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bvk.epnwcf.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xqi.ctjpmb.com

[E06] 替换子串
来源：http://jke.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qkh.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://zjb.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rob.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://bcn.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zlx.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fiy.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rwh.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://frn.meibo888.top

[E07] 按分隔符拆分
来源：http://jiu.gotoacloud.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ehf.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vzg.0kj1m.cn


<!-- 参考信息 -->