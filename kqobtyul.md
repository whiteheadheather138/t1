代发 wailian999

PHP:  // 无重载
来源：http://byf.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ukl.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://sri.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mwe.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://blt.cqqwz.cn

Ruby: # 无重载：靠动态参数
来源：http://kxa.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tgm.iojbl.cn

================================================================================
来源：http://tkx.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://ehu.vqdsnc.cn

================================================================================
来源：http://zdz.shzxlz.cn

[D01] 创建数组 / 列表
来源：http://vfr.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gjd.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lsj.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kzq.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ylf.pycfn.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mvo.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://gkq.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://nhx.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rkl.yuxming.cn

[D02] 追加元素到末尾
来源：http://zvy.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qdb.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://znx.nanxinkj.top

JS:   arr.push(4);
来源：http://bht.yuanzhike.top

TS:   arr.push(4);
来源：http://hej.zhixingplan.top

Java: list.add(4);
来源：http://ire.316326.xyz

Go:   arr = append(arr, 4)
来源：http://wws.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://dhw.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://uaw.hnqzz.top

[D03] 在指定位置插入元素
来源：http://hoa.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://akl.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fyh.yj20258.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yef.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://rjq.yonumen.top

Java: list.add(0, 0);
来源：http://ssu.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://egi.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lbe.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://brk.uphjek.com

[D04] 删除元素
来源：http://lgp.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vch.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cpl.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qhw.tarul.cn

TS:   arr.splice(0, 1);
来源：http://wzz.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vpu.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://esp.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rdn.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fdn.tian-w.cn

[D05] 访问与修改元素
来源：http://eyi.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ntj.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vqc.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wuv.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://fyc.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://mcc.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://uqs.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dlz.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gqb.epnwcf.com

[D06] 数组长度
来源：http://fxh.zhengqikj.top

Py:   len(arr)
来源：http://ium.yangfankeji.com

PHP:  count($arr);
来源：http://tmp.hcnkem.com

JS:   arr.length
来源：http://gfc.yueranfly.top

TS:   arr.length
来源：http://onc.aizwys.cn

Java: list.size();
来源：http://clo.hnqzz.top

Go:   len(arr)
来源：http://trs.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://hbp.zhiwuduotai.top

C#:   list.Count;
来源：http://qbo.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://udd.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mkh.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iud.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://zam.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://edj.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://wcn.dianchejie.cn

Go:   arr[1:4]
来源：http://rns.jinqigufen.top

Ruby: arr[1, 3]
来源：http://aso.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://qwh.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://ldo.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://hna.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://gfi.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tnp.yuanzhike.top

TS:   [...a, ...b];
来源：http://hjj.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bub.shzxlz.cn

Go:   append(a, b...)
来源：http://lmj.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://bbl.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://gxk.jyoumei.cn

[D09] 排序（升序）
来源：http://zuz.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://ecc.hnqzz.top

PHP:  sort($arr);
来源：http://uxw.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xnh.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oyd.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://hxj.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fbp.cheryme.top

Ruby: arr.sort
来源：http://xoo.yanxiufei.cn

C#:   list.Sort();
来源：http://hzl.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dsn.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xyi.cucudq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vxh.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fjo.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yzj.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mec.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://unb.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eic.hongshengwenyu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bpw.havefunace.top

[D11] 反转数组
来源：http://nqw.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://uyv.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://uit.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qyi.meibo888.top

TS:   [...arr].reverse();
来源：http://now.hammf.cn

Java: Collections.reverse(list);
来源：http://xbr.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://qyb.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://kvi.birdmap.top

C#:   list.Reverse();
来源：http://jlk.dashuyun.cn

[D12] 查找元素下标
来源：http://owp.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://dqh.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gfg.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hnh.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fbw.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lwf.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://ajs.gaohongyu789.top

Ruby: arr.index(x)
来源：http://pgk.daria6918.cn

C#:   list.IndexOf(x);
来源：http://sji.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://mkf.zdbjq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bqq.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yza.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://sbi.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://qlg.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yvj.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wgt.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ipt.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bgl.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://opm.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://prj.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jte.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://pgo.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://xas.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mme.yuanzhike.top

Go:   // 手写循环
来源：http://oen.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://tel.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gtv.hnxiangtu.top

[D15] 去重
来源：http://pgn.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dop.ivvv.top

PHP:  array_unique($arr);
来源：http://kmz.zycfv.cn

JS:   [...new Set(arr)]
来源：http://zoq.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://vjp.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kbp.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://qqs.dashuyun.cn

Ruby: arr.uniq
来源：http://mtr.c1oappe.top

C#:   list.Distinct().ToList()
来源：http://icf.nanxinkj.top

[D16] 求和与平均值
来源：http://mfd.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://efg.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tdc.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lke.quarkkingdee.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mgg.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ujf.aizwys.cn

Go:   // 手写循环累加
来源：http://hqu.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qpw.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://pcu.yangfankeji.com

[D17] 最大值与最小值
来源：http://xos.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://mvh.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://awa.shuidangran.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dgl.zhixingplan.top

TS:   Math.max(...arr);
来源：http://pbk.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mtr.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tpl.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://ysb.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://xnq.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://sjh.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sps.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://mds.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pgv.xinyue.icu

TS:   nested.flat();
来源：http://nhh.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cjc.shuidangran.top

Go:   // 手写双层循环
来源：http://rvo.jyoumei.cn

Ruby: nested.flatten
来源：http://siy.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://phn.haohaochexian.top

[D19] 按字段分组
来源：http://dje.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wfx.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zls.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ase.jyoumei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vum.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jlz.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://stx.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lyq.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fix.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://rlo.yongpay.top

Py:   Counter(arr)
来源：http://wpg.daxiang520.top

PHP:  array_count_values($arr);
来源：http://yyl.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://muh.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://liq.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dun.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://hzs.52xcode.cn

Ruby: arr.tally
来源：http://ppy.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zot.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://xfc.andypj.xyz

Py:   x in arr
来源：http://uev.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://dyl.zdbjq.cn

JS:   arr.includes(x)
来源：http://dvg.havefunace.top

TS:   arr.includes(x)
来源：http://hsv.epnwcf.com

Java: list.contains(x)
来源：http://aag.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://imz.cashguo.top

Ruby: arr.include?(x)
来源：http://ggs.mhx1999.top

C#:   list.Contains(x)
来源：http://cgk.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://tsb.smart0.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ntn.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tju.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hsb.shanyushiyangkeji.top

TS:   [...arr];
来源：http://mik.yvedp.cn

Java: new ArrayList<>(list);
来源：http://mli.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zwq.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://esf.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://vob.0kj1m.cn

[D23] reduce 累积计算
来源：http://cht.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://clx.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dop.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uhg.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bwk.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qto.yvedp.cn

Go:   // 手写循环
来源：http://ytq.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pyj.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ohy.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://rec.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qqb.tanke756.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://weg.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jer.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yfl.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ezp.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jow.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jpq.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xaz.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://lmz.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tlj.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mun.316326.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xts.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hhn.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://shx.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iun.hesvh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://loj.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mrv.dashuyun.cn

[D26] 数组转字符串
来源：http://cbc.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://gup.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://usc.iojbl.cn

JS:   arr.join(", ")
来源：http://qah.cheryme.top

TS:   arr.join(", ")
来源：http://sxt.hysaishi.cn

Java: String.join(", ", list)
来源：http://zhb.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://cna.hcnkem.com

Ruby: arr.join(", ")
来源：http://orc.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://cnl.nanxinkj.top

================================================================================
来源：http://ezz.sweek.top

E. 字符串处理
来源：http://ijl.vehdjk.com

================================================================================
来源：http://iuv.c1oappe.top

[E01] 拼接字符串
来源：http://chb.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uhq.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qoo.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pod.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hbw.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kde.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xki.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://urf.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wct.c1oappe.top

[E02] 重复字符串
来源：http://rbl.guowangkeji.top

Py:   "ab" * 3
来源：http://trq.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://oop.cucudq.cn

JS:   "ab".repeat(3)
来源：http://wui.bjfxy.top

TS:   "ab".repeat(3)
来源：http://zox.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://eal.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://fyc.gotoacloud.top

Ruby: "ab" * 3
来源：http://kaz.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ozb.jinqigfzy.top

[E03] 截取子串
来源：http://cyh.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://okh.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://utf.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bcp.iojbl.cn

TS:   s.slice(1, 4)
来源：http://zfd.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://eol.316326.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jtx.tian-w.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fna.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://jbg.yj20258.top

[E04] 查找子串位置
来源：http://idt.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://cua.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://wmg.cashguo.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kty.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://ogg.316326.xyz

Java: s.indexOf("x")
来源：http://rud.jqgfzy.top

Go:   strings.Index(s, "x")
来源：http://awb.hesvh.cn

Ruby: s.index("x")
来源：http://cwq.ivvv.top

C#:   s.IndexOf("x")
来源：http://jxs.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hzn.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ecj.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kka.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gne.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vcp.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://izy.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qte.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zuq.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zfk.yangfankeji.com

[E06] 替换子串
来源：http://ykw.cucudq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ann.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://yky.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kml.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://ihk.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://puv.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zyu.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fin.cheryme.top


<!-- 参考信息 -->