代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://rcs.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://vig.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://enr.tian-w.cn

================================================================================
来源：http://upf.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://rxd.zhongyouzk.top

================================================================================
来源：http://wuu.jianghu66.top

[D01] 创建数组 / 列表
来源：http://trw.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iij.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dhu.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wxm.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://krd.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hgu.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://nfw.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://cde.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ckx.hysaishi.cn

[D02] 追加元素到末尾
来源：http://vaa.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hfm.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bgc.birdmap.top

JS:   arr.push(4);
来源：http://oii.hfpthk.cn

TS:   arr.push(4);
来源：http://vjn.bbcook.cn

Java: list.add(4);
来源：http://mlk.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://djd.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://msk.yanxiufei.cn

C#:   list.Add(4);
来源：http://uly.jqgufenzy.top

[D03] 在指定位置插入元素
来源：http://hai.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://gfa.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uxc.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bln.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://wfq.sxryk.cn

Java: list.add(0, 0);
来源：http://dqv.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dif.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mgb.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://kih.zdqjudy.top

[D04] 删除元素
来源：http://ydy.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kmq.hesvh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jpm.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lsa.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://vbi.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ped.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uiw.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hyy.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vjl.nanxinkj.top

[D05] 访问与修改元素
来源：http://mvo.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ypj.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fbw.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jke.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://poz.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://ydl.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://nzd.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vfx.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jjq.ydjk.org.cn

[D06] 数组长度
来源：http://xjz.tianlin.xyz

Py:   len(arr)
来源：http://acf.sweek.top

PHP:  count($arr);
来源：http://knm.fehbvm.com

JS:   arr.length
来源：http://hit.uphjek.com

TS:   arr.length
来源：http://ayd.havefunace.top

Java: list.size();
来源：http://vcz.chenzaomai.com

Go:   len(arr)
来源：http://dup.fengsongda.top

Ruby: arr.length; arr.size
来源：http://ykf.wangshuangyany.cn

C#:   list.Count;
来源：http://jxp.meibo888.top

[D07] 切片 / 取子数组
来源：http://bxz.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lht.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://jha.sweek.top

JS:   arr.slice(1, 4);
来源：http://rud.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://gfh.zdqjudy.top

Java: list.subList(1, 4);
来源：http://ils.jlsjyb.cn

Go:   arr[1:4]
来源：http://eox.iojbl.cn

Ruby: arr[1, 3]
来源：http://ywe.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://yql.c1oappe.top

[D08] 合并两个数组
来源：http://zoy.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://moy.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://jjw.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gcu.cucudq.cn

TS:   [...a, ...b];
来源：http://czf.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zfj.jianghu66.top

Go:   append(a, b...)
来源：http://lkn.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://yeg.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://gak.hcnkem.com

[D09] 排序（升序）
来源：http://yfx.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://pqw.tarul.cn

PHP:  sort($arr);
来源：http://kil.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xhr.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wsx.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://qcb.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sgg.hnqzz.top

Ruby: arr.sort
来源：http://vzr.gogol.net.cn

C#:   list.Sort();
来源：http://cbo.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://svg.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vbj.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lkp.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jes.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nbw.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dem.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wdk.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nte.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dow.jianghu66.top

[D11] 反转数组
来源：http://veu.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://zdu.gzhubu.top

PHP:  array_reverse($arr);
来源：http://fiv.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qzf.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://wwt.fzhhl.top

Java: Collections.reverse(list);
来源：http://sfr.hammf.cn

Go:   slices.Reverse(arr)
来源：http://bsz.dashuyun.cn

Ruby: arr.reverse
来源：http://ybt.bbcook.cn

C#:   list.Reverse();
来源：http://ihf.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://yhu.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://kej.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bfu.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kwb.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://skn.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kgd.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://ldy.yj20258888.top

Ruby: arr.index(x)
来源：http://tpn.daxiang520.top

C#:   list.IndexOf(x);
来源：http://afm.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://nre.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kzw.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qxt.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://hhn.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://pox.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://knq.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ery.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ebp.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://wjx.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://dkc.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ock.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fyu.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://vjy.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://wla.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://etp.yj202588.top

Go:   // 手写循环
来源：http://ykb.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lxf.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://fxh.c1oappe.top

[D15] 去重
来源：http://fxm.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ost.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://fhk.redwolf501.top

JS:   [...new Set(arr)]
来源：http://vta.cheryme.top

TS:   [...new Set(arr)]
来源：http://wjs.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wud.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://okl.snrcjt.cn

Ruby: arr.uniq
来源：http://xth.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://utw.havefunace.top

[D16] 求和与平均值
来源：http://uzr.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vdr.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uby.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ewm.smart0.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gxk.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ahu.aibaodan.cn

Go:   // 手写循环累加
来源：http://ksw.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vvq.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://bpm.zhongyouzk.top

[D17] 最大值与最小值
来源：http://lpc.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://kon.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://hzx.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aov.52xcode.cn

TS:   Math.max(...arr);
来源：http://nou.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gks.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cvt.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://nkm.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://awz.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://byj.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jmm.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://rwu.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://frc.sufxvd.cn

TS:   nested.flat();
来源：http://wul.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://otn.jqgfzy.top

Go:   // 手写双层循环
来源：http://iyj.kuanghao11.cn

Ruby: nested.flatten
来源：http://wsy.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hoi.hnxiangtu.top

[D19] 按字段分组
来源：http://yjw.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bfw.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dtk.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hwk.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pif.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uyc.cashguo.top

Go:   // 手写 map[string][]T
来源：http://coy.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://cnl.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yig.sxryk.cn

[D20] 统计每个元素出现次数
来源：http://uwa.sufxvd.cn

Py:   Counter(arr)
来源：http://yvp.shuidangran.top

PHP:  array_count_values($arr);
来源：http://uir.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kge.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://htm.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ntl.cucudq.cn

Go:   // 手写 map[T]int
来源：http://eit.hfpthk.cn

Ruby: arr.tally
来源：http://dpt.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dey.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://dzk.svipenyu.cn

Py:   x in arr
来源：http://eat.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://oan.ppjwa.cn

JS:   arr.includes(x)
来源：http://djs.nwbrower.top

TS:   arr.includes(x)
来源：http://icp.ydjk.org.cn

Java: list.contains(x)
来源：http://ttv.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://dao.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://ggk.316326.xyz

C#:   list.Contains(x)
来源：http://gqf.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://fvh.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ofh.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kkg.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://orp.gzhubu.top

TS:   [...arr];
来源：http://gys.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://yld.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tym.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://apb.haohaochexian.top

C#:   new List<int>(list);
来源：http://nfm.yuanzhike.top

[D23] reduce 累积计算
来源：http://jlw.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vgm.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pkb.redwolf501.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mdp.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fsm.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rer.iojbl.cn

Go:   // 手写循环
来源：http://uns.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rrz.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://skq.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://pnz.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ots.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vpt.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mwp.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fbu.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ghf.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rnt.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qjf.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pud.hnqzz.top

[D25] Set 集合去重与交并差
来源：http://stt.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lty.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yvl.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pxn.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gsr.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cqf.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zlc.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gdk.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pra.chenlongwang.top

[D26] 数组转字符串
来源：http://uln.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://ucw.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://yig.aizwys.cn

JS:   arr.join(", ")
来源：http://stu.tarul.cn

TS:   arr.join(", ")
来源：http://ilf.9152youxi.cn

Java: String.join(", ", list)
来源：http://tsc.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://bpb.xylfe.cn

Ruby: arr.join(", ")
来源：http://thk.uphjek.com

C#:   string.Join(", ", list)
来源：http://oeo.jinyuanbaomall.cn

================================================================================
来源：http://hoz.zdqjudy.top

E. 字符串处理
来源：http://his.xuetiantiany.cn

================================================================================
来源：http://vtm.aibaodan.cn

[E01] 拼接字符串
来源：http://ciz.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://emb.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ucn.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nwe.yfazqb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxj.fehbvm.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lqi.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://loi.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ngk.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tqd.jlsjyb.cn

[E02] 重复字符串
来源：http://ogy.dashuyun.cn

Py:   "ab" * 3
来源：http://eau.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://bmn.birdmap.top

JS:   "ab".repeat(3)
来源：http://fbi.guannengcc.top

TS:   "ab".repeat(3)
来源：http://uvb.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://ufg.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://mxl.c1oappe.top

Ruby: "ab" * 3
来源：http://fob.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://olq.ybcxt.top

[E03] 截取子串
来源：http://oab.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ead.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uld.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://suz.daria6918.cn

TS:   s.slice(1, 4)
来源：http://agk.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://eyl.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jjv.cdnleiting.top

Ruby: s[1, 3];  s[1..3]
来源：http://avq.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://nlk.havefunace.top

[E04] 查找子串位置
来源：http://jls.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://vff.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://lfj.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aph.fzhhl.top

TS:   s.indexOf("x")
来源：http://tgp.yanxiufei.cn

Java: s.indexOf("x")
来源：http://uqa.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://zss.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://mdf.cucudq.cn

C#:   s.IndexOf("x")
来源：http://knn.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bbs.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qcz.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ltt.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zxs.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qfp.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lfm.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wkq.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vog.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ezx.epnwcf.com

[E06] 替换子串
来源：http://pqc.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uxg.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://qkh.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dpv.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://qxx.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wcj.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://naq.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qji.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://jmd.snrcjt.cn

[E07] 按分隔符拆分
来源：http://nkc.guannengcc.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cts.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://atv.gotoacloud.top


<!-- 参考信息 -->