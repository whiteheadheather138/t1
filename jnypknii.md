代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://mde.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://zgy.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kos.yangfankeji.com

================================================================================
来源：http://sys.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://qdm.vqdsnc.cn

================================================================================
来源：http://ohi.fehbvm.com

[D01] 创建数组 / 列表
来源：http://jrt.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dvk.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kjm.ydjk.org.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xkk.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nku.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lie.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://agh.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://btf.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zib.jianghu66.top

[D02] 追加元素到末尾
来源：http://owq.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vfv.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wvv.vqdsnc.cn

JS:   arr.push(4);
来源：http://fvw.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://atu.dianchejie.cn

Java: list.add(4);
来源：http://nzd.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://agx.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://ezl.wangshuangyany.cn

C#:   list.Add(4);
来源：http://ugg.52xcode.cn

[D03] 在指定位置插入元素
来源：http://thz.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://ouq.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rxi.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iuo.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://tir.ivvv.top

Java: list.add(0, 0);
来源：http://cri.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://xsz.hesvh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vcn.kuanghao11.cn

C#:   list.Insert(0, 0);
来源：http://ksj.hywenlv.cn

[D04] 删除元素
来源：http://gow.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xxc.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oac.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kwb.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://kbz.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ttq.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dgz.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kud.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sqm.jianghu66.top

[D05] 访问与修改元素
来源：http://baj.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sok.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jge.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ocj.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://xgn.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://nqk.jyoumei.cn

Go:   arr[0]; arr[0] = 9
来源：http://mgb.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eiw.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uev.shzxlz.cn

[D06] 数组长度
来源：http://cly.daxiang520.top

Py:   len(arr)
来源：http://ogc.nanxuanxn.top

PHP:  count($arr);
来源：http://rna.chenlongwang.top

JS:   arr.length
来源：http://wmb.ybcxt.top

TS:   arr.length
来源：http://gtk.jinghuilouyu.cn

Java: list.size();
来源：http://azi.dianchejie.cn

Go:   len(arr)
来源：http://wzd.yj202588.top

Ruby: arr.length; arr.size
来源：http://fii.shzxlz.cn

C#:   list.Count;
来源：http://nbf.cucudq.cn

[D07] 切片 / 取子数组
来源：http://zao.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://was.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://hoe.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://xfm.hammf.cn

TS:   arr.slice(1, 4);
来源：http://ipk.nwbrower.top

Java: list.subList(1, 4);
来源：http://mhw.zycfv.cn

Go:   arr[1:4]
来源：http://nsf.dianchejie.cn

Ruby: arr[1, 3]
来源：http://zpz.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://ryf.jiagoushi.top

[D08] 合并两个数组
来源：http://ebs.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://kjx.ivvv.top

PHP:  array_merge($a, $b);
来源：http://xci.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://czl.zdqjudy.top

TS:   [...a, ...b];
来源：http://mtf.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bca.sweek.top

Go:   append(a, b...)
来源：http://jbg.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://zrq.sweek.top

C#:   a.Concat(b).ToList()
来源：http://pej.tian-w.cn

[D09] 排序（升序）
来源：http://phe.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://iuj.zhiwuduotai.top

PHP:  sort($arr);
来源：http://ihw.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wgb.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qou.xuetiantiany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://csp.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kmi.yj20258.top

Ruby: arr.sort
来源：http://xeg.redwolf501.top

C#:   list.Sort();
来源：http://ymp.redwolf501.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nrc.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cax.fzhhl.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iwu.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fxn.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uzo.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vch.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ufa.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tsl.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://umh.hongshengwenyu.top

[D11] 反转数组
来源：http://ruf.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ykf.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://low.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mop.xziqi.cn

TS:   [...arr].reverse();
来源：http://ucw.9152youxi.cn

Java: Collections.reverse(list);
来源：http://gir.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://dta.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://gqb.haohaochexian.top

C#:   list.Reverse();
来源：http://qks.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://jtf.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://dqh.nwbrower.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://apn.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jbk.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehp.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lia.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://cmo.jqgufenzy.top

Ruby: arr.index(x)
来源：http://mhi.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://gal.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://ysx.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kmr.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oxe.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://edf.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://bxc.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ygq.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lat.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://igy.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rii.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://uud.fktsv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oga.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iyw.gotoacloud.top

JS:   arr.map(x => x * 2)
来源：http://jzh.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://vzw.yj20258888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rtx.jyoumei.cn

Go:   // 手写循环
来源：http://lcv.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://byb.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eei.jinghuilouyu.cn

[D15] 去重
来源：http://vko.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://maj.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://bsy.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://vhe.yuxming.cn

TS:   [...new Set(arr)]
来源：http://dak.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://spw.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bav.jqgufenzy.top

Ruby: arr.uniq
来源：http://fdk.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://lqv.epnwcf.com

[D16] 求和与平均值
来源：http://ljy.quarkkingdee.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ugy.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qtv.tian-w.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cbh.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kpg.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vwm.shuidangran.top

Go:   // 手写循环累加
来源：http://vww.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eci.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://dfq.gogol.net.cn

[D17] 最大值与最小值
来源：http://xhn.316326.xyz

Py:   max(arr);  min(arr)
来源：http://ctx.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://eqh.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ape.yvedp.cn

TS:   Math.max(...arr);
来源：http://xjg.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gvo.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pyh.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://vae.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://nro.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://bqd.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pfw.cheryme.top

PHP:  array_merge(...$nested);
来源：http://oxd.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sjh.tarul.cn

TS:   nested.flat();
来源：http://voc.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ydr.gotoacloud.top

Go:   // 手写双层循环
来源：http://utk.feifeiyinyue.top

Ruby: nested.flatten
来源：http://xah.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ejc.9152youxi.cn

[D19] 按字段分组
来源：http://lpp.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gsl.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wup.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ylx.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pgv.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qdv.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://fwi.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wmg.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gyt.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://hap.andypj.xyz

Py:   Counter(arr)
来源：http://ziw.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://fxp.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uws.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yxw.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cjl.hesvh.cn

Go:   // 手写 map[T]int
来源：http://vtz.tanke756.top

Ruby: arr.tally
来源：http://xlr.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xdz.yonumen.top

[D21] 判断是否包含某元素
来源：http://ccx.havefunace.top

Py:   x in arr
来源：http://sbr.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://nzx.fktsv.cn

JS:   arr.includes(x)
来源：http://upi.zhoulong.xyz

TS:   arr.includes(x)
来源：http://gke.fktsv.cn

Java: list.contains(x)
来源：http://hcx.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://rsl.yj202588.top

Ruby: arr.include?(x)
来源：http://rop.jqgufenzy.top

C#:   list.Contains(x)
来源：http://opm.xingfuxueyuan.xyz

[D22] 复制数组（避免共享引用）
来源：http://obg.hysaishi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lxf.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vko.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vyz.cashguo.top

TS:   [...arr];
来源：http://aee.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://wro.wangshuangyany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://shm.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://ahh.shzxlz.cn

C#:   new List<int>(list);
来源：http://gtp.cdnleiting.top

[D23] reduce 累积计算
来源：http://tyc.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xqn.jiagoushi.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pqf.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tay.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mbp.zdbjq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oxz.sxryk.cn

Go:   // 手写循环
来源：http://iau.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qlx.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gyy.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://vqo.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jje.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eac.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qqu.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aiz.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lvp.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pdi.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ikr.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pnw.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://xjz.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://byi.zdqjudy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zpi.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iaa.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qts.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tmq.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xvs.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qfu.zycfv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zgr.ydjk.org.cn

[D26] 数组转字符串
来源：http://tro.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://vzd.sweek.top

PHP:  implode(", ", $arr);
来源：http://qaa.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://qvi.nanxinkj.top

TS:   arr.join(", ")
来源：http://vsu.yuxming.cn

Java: String.join(", ", list)
来源：http://nup.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://xlm.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://xkl.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://jhx.ybcxt.top

================================================================================
来源：http://ppb.fzhhl.top

E. 字符串处理
来源：http://xjf.nanxuanxn.top

================================================================================
来源：http://kjv.zhixingplan.top

[E01] 拼接字符串
来源：http://ihy.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fsb.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vnp.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://prf.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hxq.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rey.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ayh.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lru.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wfd.hysaishi.cn

[E02] 重复字符串
来源：http://jjh.ivvv.top

Py:   "ab" * 3
来源：http://rmr.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://yzp.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://cbq.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://saj.fktsv.cn

Java: "ab".repeat(3)
来源：http://aqt.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://ode.birdmap.top

Ruby: "ab" * 3
来源：http://wms.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fvh.zhixingplan.top

[E03] 截取子串
来源：http://puz.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sew.wangdashe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pvi.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ppe.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://yny.cashguo.top

Java: s.substring(1, 4)
来源：http://lqm.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://clc.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bll.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://fsd.andypj.xyz

[E04] 查找子串位置
来源：http://xhu.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://lak.fzhhl.top

PHP:  strpos($s, "x");
来源：http://crs.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://emg.meibo888.top

TS:   s.indexOf("x")
来源：http://ljm.c1oappe.top

Java: s.indexOf("x")
来源：http://yxm.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://yru.nanxinkj.top

Ruby: s.index("x")
来源：http://ioc.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://wkj.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://age.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rfw.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hzk.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wmq.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zwu.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yym.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yeu.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xtt.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gsq.nwbrower.top

[E06] 替换子串
来源：http://att.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uet.yanxiufei.cn

PHP:  str_replace("a", "b", $s);
来源：http://ews.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mud.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://hrs.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aww.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pjz.sufxvd.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wtp.yj202588.top

C#:   s.Replace("a", "b")
来源：http://nul.tianlin.xyz

[E07] 按分隔符拆分
来源：http://pie.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zvi.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bcg.jqgfzy.top


<!-- 参考信息 -->