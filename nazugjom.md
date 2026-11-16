代发 wailian999

PHP:  // 无重载
来源：http://acy.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jqt.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://ssg.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://udc.zhijiandao.cn

Go:   // 无重载：用不同函数名
来源：http://rjg.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://oht.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jyz.ppjwa.cn

================================================================================
来源：http://hag.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://xbb.jianghu66.top

================================================================================
来源：http://rum.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://vfo.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://was.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bvw.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hrs.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://rco.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xvo.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://fxc.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://hot.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pdp.jqgfzy.top

[D02] 追加元素到末尾
来源：http://aod.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wwq.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kqm.yongpay.top

JS:   arr.push(4);
来源：http://vdn.yj20258888.top

TS:   arr.push(4);
来源：http://xsz.redwolf501.top

Java: list.add(4);
来源：http://nvo.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://dwy.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://qgz.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://kbj.tian-w.cn

[D03] 在指定位置插入元素
来源：http://fap.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://tdt.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nym.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://okq.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://zky.jqgfzy.top

Java: list.add(0, 0);
来源：http://brt.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zpi.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gzg.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://rnw.andypj.xyz

[D04] 删除元素
来源：http://xth.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pqd.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ihi.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kbq.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://igt.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://knt.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://djz.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ygg.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ohu.jqgufenzy.top

[D05] 访问与修改元素
来源：http://nol.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zij.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://efr.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rxp.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://ihu.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://qar.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://fdm.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vbk.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kbd.zhoulong.xyz

[D06] 数组长度
来源：http://rxz.jianghu66.top

Py:   len(arr)
来源：http://qce.hnxiangtu.top

PHP:  count($arr);
来源：http://iei.mhx1999.top

JS:   arr.length
来源：http://mav.ehwqpu.com

TS:   arr.length
来源：http://oct.gotoacloud.top

Java: list.size();
来源：http://bym.52xcode.cn

Go:   len(arr)
来源：http://osy.tian-w.cn

Ruby: arr.length; arr.size
来源：http://zbz.yongpay.top

C#:   list.Count;
来源：http://qwt.fehbvm.com

[D07] 切片 / 取子数组
来源：http://rkw.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tia.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://obq.yongpay.top

JS:   arr.slice(1, 4);
来源：http://pqe.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://yhh.aizwys.cn

Java: list.subList(1, 4);
来源：http://szw.zdqjudy.top

Go:   arr[1:4]
来源：http://xgm.hywenlv.cn

Ruby: arr[1, 3]
来源：http://yqd.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://nve.xziqi.cn

[D08] 合并两个数组
来源：http://hej.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://xob.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://sqf.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://keb.ppjwa.cn

TS:   [...a, ...b];
来源：http://roh.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hww.yuanzhike.top

Go:   append(a, b...)
来源：http://ort.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://hzw.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://zcp.hongshengwenyu.top

[D09] 排序（升序）
来源：http://uii.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://imb.daxiang520.top

PHP:  sort($arr);
来源：http://myj.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gxe.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://unl.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://lqk.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vok.cashguo.top

Ruby: arr.sort
来源：http://qjd.fzhhl.top

C#:   list.Sort();
来源：http://xok.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rng.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vsl.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pnr.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyr.nwbrower.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfz.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bos.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mbz.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://toe.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xop.jqgufenzy.top

[D11] 反转数组
来源：http://ofr.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://qoh.tanke756.top

PHP:  array_reverse($arr);
来源：http://wfk.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pdm.yuxming.cn

TS:   [...arr].reverse();
来源：http://duj.xziqi.cn

Java: Collections.reverse(list);
来源：http://ctl.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://dij.shangyingyoupin.top

Ruby: arr.reverse
来源：http://awp.yongpay.top

C#:   list.Reverse();
来源：http://ofl.yuxming.cn

[D12] 查找元素下标
来源：http://rhm.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://mtx.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gtw.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ikh.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qop.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bap.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://ome.gotoacloud.top

Ruby: arr.index(x)
来源：http://fde.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://uvh.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://vbn.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rwg.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xjm.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://trf.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://uyg.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yba.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xzh.cashguo.top

Ruby: arr.select { |x| x > 3 }
来源：http://nku.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://hwf.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://tlc.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kae.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://czh.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://dao.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://bvm.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jlf.yangfankeji.com

Go:   // 手写循环
来源：http://pms.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://wnz.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dan.zdqjudy.top

[D15] 去重
来源：http://gus.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://obz.nanxinkj.top

PHP:  array_unique($arr);
来源：http://nxt.tian-w.cn

JS:   [...new Set(arr)]
来源：http://akw.daxiang520.top

TS:   [...new Set(arr)]
来源：http://scy.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://voo.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://lpf.hcnkem.com

Ruby: arr.uniq
来源：http://tve.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://rug.chenlongwang.top

[D16] 求和与平均值
来源：http://hkj.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qiz.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wly.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ibq.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fkv.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wxf.yueranfly.top

Go:   // 手写循环累加
来源：http://yto.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zny.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://obm.chenlongwang.top

[D17] 最大值与最小值
来源：http://esu.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://tck.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://ujz.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kpz.xziqi.cn

TS:   Math.max(...arr);
来源：http://kwh.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xty.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xke.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://qmt.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://ayo.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://nuv.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oyp.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://hbs.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fop.yangfankeji.com

TS:   nested.flat();
来源：http://aoa.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://naf.epnwcf.com

Go:   // 手写双层循环
来源：http://nzg.havefunace.top

Ruby: nested.flatten
来源：http://kgg.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://naf.0kj1m.cn

[D19] 按字段分组
来源：http://fak.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jbq.zhiwuduotai.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yqe.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vju.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rjd.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tkd.yj20258.top

Go:   // 手写 map[string][]T
来源：http://bub.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zkv.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://coi.meibo888.top

[D20] 统计每个元素出现次数
来源：http://wmx.cqqwz.cn

Py:   Counter(arr)
来源：http://gye.smart0.xyz

PHP:  array_count_values($arr);
来源：http://pba.bjfxy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sxs.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dcq.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wfr.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://phi.ctjpmb.com

Ruby: arr.tally
来源：http://lnu.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lxg.aizwys.cn

[D21] 判断是否包含某元素
来源：http://uyv.hywenlv.cn

Py:   x in arr
来源：http://tna.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://gcm.gogol.net.cn

JS:   arr.includes(x)
来源：http://atq.jianghu66.top

TS:   arr.includes(x)
来源：http://gwe.jinghuilouyu.cn

Java: list.contains(x)
来源：http://edl.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://hjo.yj20258888.top

Ruby: arr.include?(x)
来源：http://kgb.52xcode.cn

C#:   list.Contains(x)
来源：http://eea.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://rcc.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wrg.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nuj.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gni.ydzc1.top

TS:   [...arr];
来源：http://gcc.redwolf501.top

Java: new ArrayList<>(list);
来源：http://zjy.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://esz.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://ivk.bjfxy.top

C#:   new List<int>(list);
来源：http://ydg.shuidangran.top

[D23] reduce 累积计算
来源：http://ogk.yuanzhike.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mnk.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mmg.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://idl.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qjn.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xto.fktsv.cn

Go:   // 手写循环
来源：http://cjd.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pra.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ipr.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://cxg.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gai.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lee.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dwr.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iaj.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cad.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gzu.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://djj.xinyue.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nuo.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://yyh.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ubj.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cph.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zfw.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://onq.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sdt.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nvd.shuidangran.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nxc.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zhj.ppjwa.cn

[D26] 数组转字符串
来源：http://atr.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://nlb.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://yfl.redwolf501.top

JS:   arr.join(", ")
来源：http://vjx.9152youxi.cn

TS:   arr.join(", ")
来源：http://yvz.snrcjt.cn

Java: String.join(", ", list)
来源：http://cqm.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://pjo.chenzaomai.com

Ruby: arr.join(", ")
来源：http://eiz.pycfn.com

C#:   string.Join(", ", list)
来源：http://myb.smart0.xyz

================================================================================
来源：http://gmc.epnwcf.com

E. 字符串处理
来源：http://emj.mhx1999.top

================================================================================
来源：http://cdb.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://jhv.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bhg.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zxp.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mct.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://umf.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ywk.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ohg.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cxh.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fhm.xuanzx.com

[E02] 重复字符串
来源：http://iaw.jinqigufen.top

Py:   "ab" * 3
来源：http://lor.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://uhy.xziqi.cn

JS:   "ab".repeat(3)
来源：http://hun.yj20258888.top

TS:   "ab".repeat(3)
来源：http://dxh.uphjek.com

Java: "ab".repeat(3)
来源：http://nay.zhaomingkeji.xyz

Go:   strings.Repeat("ab", 3)
来源：http://keb.yj20258888.top

Ruby: "ab" * 3
来源：http://iax.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jqi.fanxiaobao.xyz

[E03] 截取子串
来源：http://fig.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yni.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iry.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvk.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://ynb.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://xcy.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nef.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://cqm.meibo888.top

C#:   s.Substring(1, 3)
来源：http://ldk.zhiwuduotai.top

[E04] 查找子串位置
来源：http://zwe.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://bdq.hnxiangtu.top

PHP:  strpos($s, "x");
来源：http://glt.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ajl.mhx1999.top

TS:   s.indexOf("x")
来源：http://tte.pycfn.com

Java: s.indexOf("x")
来源：http://itd.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://ilb.ydzc1.top

Ruby: s.index("x")
来源：http://uia.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://ftk.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gix.dashuyun.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jsm.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vbm.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xjy.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cky.jyoumei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mrx.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://slm.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yes.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ilp.gogol.net.cn

[E06] 替换子串
来源：http://bbl.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bgd.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://umn.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ikq.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://xtb.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://emg.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nmh.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xxt.tianlin.xyz


<!-- 参考信息 -->