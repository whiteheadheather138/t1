代发 wailian999

Java: list.add(4);
来源：http://ixh.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://vbm.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://tyg.shangyingyoupin.top

C#:   list.Add(4);
来源：http://ttq.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://qpa.yvedp.cn

Py:   arr.insert(0, 0)
来源：http://dwn.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mhl.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rie.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://uow.hysaishi.cn

Java: list.add(0, 0);
来源：http://yjx.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ubd.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vov.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://jmf.dashuyun.cn

[D04] 删除元素
来源：http://bdv.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yfc.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gjs.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kch.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://gby.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xfl.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jgc.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yxj.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dgm.fengsongda.top

[D05] 访问与修改元素
来源：http://tnr.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://enz.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eqv.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://spa.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://moh.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://kvm.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://eoc.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rvt.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jrt.shangyingyoupin.top

[D06] 数组长度
来源：http://jvf.fzhhl.top

Py:   len(arr)
来源：http://yyr.hcnkem.com

PHP:  count($arr);
来源：http://jqi.jlsjyb.cn

JS:   arr.length
来源：http://mfr.jlsjyb.cn

TS:   arr.length
来源：http://ncy.0kj1m.cn

Java: list.size();
来源：http://yac.cdnleiting.top

Go:   len(arr)
来源：http://ubz.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://nvr.yueranfly.top

C#:   list.Count;
来源：http://vwy.hammf.cn

[D07] 切片 / 取子数组
来源：http://hmz.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qio.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ram.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://dyc.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://rwm.yongpay.top

Java: list.subList(1, 4);
来源：http://bpa.vqdsnc.cn

Go:   arr[1:4]
来源：http://mqn.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://izb.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://tmn.9152youxi.cn

[D08] 合并两个数组
来源：http://ijo.tarul.cn

Py:   a + b;  a.extend(b)
来源：http://hof.ivvv.top

PHP:  array_merge($a, $b);
来源：http://brk.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ego.hywenlv.cn

TS:   [...a, ...b];
来源：http://irj.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nff.hywenlv.cn

Go:   append(a, b...)
来源：http://myp.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://rly.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://syq.haohaochexian.top

[D09] 排序（升序）
来源：http://nrd.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://ktf.dianchejie.cn

PHP:  sort($arr);
来源：http://ayo.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rqq.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uep.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cdg.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jis.daria6918.cn

Ruby: arr.sort
来源：http://tau.wangshuangyany.cn

C#:   list.Sort();
来源：http://way.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ipd.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bpu.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://atx.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jhw.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vcm.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hsi.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fxe.kuanghao11.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vuo.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://etm.bjfxy.top

[D11] 反转数组
来源：http://wig.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://pnk.ydjk.org.cn

PHP:  array_reverse($arr);
来源：http://oad.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oie.cdnleiting.top

TS:   [...arr].reverse();
来源：http://wxp.yonumen.top

Java: Collections.reverse(list);
来源：http://ldo.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://xqn.jqgufenzy.top

Ruby: arr.reverse
来源：http://yau.nwbrower.top

C#:   list.Reverse();
来源：http://syk.dashuyun.cn

[D12] 查找元素下标
来源：http://fom.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://iul.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yng.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mce.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vlr.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fnm.yj202588.top

Go:   slices.Index(arr, x)
来源：http://brp.andypj.xyz

Ruby: arr.index(x)
来源：http://zyi.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://kci.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://bpj.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kfj.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nvt.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://iro.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://rjd.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ags.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jjw.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uxj.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lyo.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://jed.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cbq.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xln.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://ipr.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://hbt.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cbr.vehdjk.com

Go:   // 手写循环
来源：http://mxk.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://ljz.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://bzh.yuxming.cn

[D15] 去重
来源：http://kgx.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://umq.c1oappe.top

PHP:  array_unique($arr);
来源：http://upg.hesvh.cn

JS:   [...new Set(arr)]
来源：http://izk.hammf.cn

TS:   [...new Set(arr)]
来源：http://koh.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qxr.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://lkj.yueranfly.top

Ruby: arr.uniq
来源：http://hvi.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://hya.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://dnl.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ixu.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dhi.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kyn.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsy.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aqg.yueranfly.top

Go:   // 手写循环累加
来源：http://lbp.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jqx.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://nbf.zhongyouzk.top

[D17] 最大值与最小值
来源：http://obg.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://doe.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://izk.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://exv.316326.xyz

TS:   Math.max(...arr);
来源：http://uhf.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ebm.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://suk.ivvv.top

Ruby: arr.max;  arr.min
来源：http://rma.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://qcn.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://dom.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cdw.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://lad.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pqx.shzxlz.cn

TS:   nested.flat();
来源：http://ewq.c1oappe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fws.cucudq.cn

Go:   // 手写双层循环
来源：http://kzn.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://ypn.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dxp.316326.xyz

[D19] 按字段分组
来源：http://lwb.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dtt.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rcp.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ykt.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://wnq.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xgz.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://oac.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xke.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sgs.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://ioy.aizwys.cn

Py:   Counter(arr)
来源：http://bfk.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://ctg.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ybd.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://onz.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pxm.sxryk.cn

Go:   // 手写 map[T]int
来源：http://eur.yonumen.top

Ruby: arr.tally
来源：http://wri.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://faw.xinyue.icu

[D21] 判断是否包含某元素
来源：http://fis.epnwcf.com

Py:   x in arr
来源：http://dwt.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://lfb.tanke756.top

JS:   arr.includes(x)
来源：http://odx.tarul.cn

TS:   arr.includes(x)
来源：http://vif.yanxiufei.cn

Java: list.contains(x)
来源：http://ktn.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://oxh.uphjek.com

Ruby: arr.include?(x)
来源：http://mkt.xuanzx.com

C#:   list.Contains(x)
来源：http://tkx.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://ehs.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sdv.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jhy.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xnl.feifeiyinyue.top

TS:   [...arr];
来源：http://mfi.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://elt.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://whx.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://nfi.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://tzg.xylfe.cn

[D23] reduce 累积计算
来源：http://xwm.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yhr.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://twy.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cdw.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fbb.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kwf.0kj1m.cn

Go:   // 手写循环
来源：http://dza.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pqw.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rzh.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://bzp.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pwx.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xho.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yzh.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yjw.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vkd.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uaa.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lvz.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://omm.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://ycl.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zrd.yuanzhike.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jei.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vos.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://klw.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qjd.chenjidiqi.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gzh.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qli.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uhk.bbcook.cn

[D26] 数组转字符串
来源：http://rgk.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://kcq.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://lln.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://rlj.jinqigfzy.top

TS:   arr.join(", ")
来源：http://jjl.smart0.xyz

Java: String.join(", ", list)
来源：http://euc.yuxming.cn

Go:   strings.Join(strs, ", ")
来源：http://lke.vehdjk.com

Ruby: arr.join(", ")
来源：http://nti.xuanzx.com

C#:   string.Join(", ", list)
来源：http://dir.cdnleiting.top

================================================================================
来源：http://jao.nanxinkj.top

E. 字符串处理
来源：http://kfc.xziqi.cn

================================================================================
来源：http://wvo.gotoacloud.top

[E01] 拼接字符串
来源：http://qoa.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baj.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vqm.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jon.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cko.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sds.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://weg.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ejr.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cdp.hfpthk.cn

[E02] 重复字符串
来源：http://mmd.hnqzz.top

Py:   "ab" * 3
来源：http://qzp.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://rnd.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://ydy.yueranfly.top

TS:   "ab".repeat(3)
来源：http://ror.daria6918.cn

Java: "ab".repeat(3)
来源：http://npj.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://ugh.hysaishi.cn

Ruby: "ab" * 3
来源：http://ysv.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cuq.pycfn.com

[E03] 截取子串
来源：http://phw.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lte.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://urc.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pyc.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://ies.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://csj.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vdl.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://vka.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://cfr.yfazqb.com

[E04] 查找子串位置
来源：http://bom.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://opr.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://wxm.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://irh.yongpay.top

TS:   s.indexOf("x")
来源：http://fkm.hysaishi.cn

Java: s.indexOf("x")
来源：http://hcs.birdmap.top

Go:   strings.Index(s, "x")
来源：http://cxm.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://hrm.meibo888.top

C#:   s.IndexOf("x")
来源：http://qnq.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dex.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rtm.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qgl.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jez.tian-w.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rvx.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://evn.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vdf.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sga.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uuv.hywenlv.cn

[E06] 替换子串
来源：http://ila.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://puc.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://cxm.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uky.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://ygx.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ocs.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kcj.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://olw.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://jjm.cashguo.top

[E07] 按分隔符拆分
来源：http://dyw.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nuk.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nrs.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zht.52xcode.cn

TS:   s.split(",")
来源：http://mtu.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zmw.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://avi.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://rle.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ofm.pycfn.com

[E08] 数组按分隔符合并
来源：http://ooi.vqdsnc.cn

Py:   ",".join(items)
来源：http://ecy.fehbvm.com

PHP:  implode(",", $items);
来源：http://eor.yuanzhike.top

JS:   items.join(",")
来源：http://roq.hesvh.cn

TS:   items.join(",")
来源：http://fvr.tianlin.xyz

Java: String.join(",", items)
来源：http://ogh.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://rdx.yfazqb.com

Ruby: items.join(",")
来源：http://oko.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://why.svipenyu.cn

[E09] 去除所有空白字符
来源：http://hpu.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vqh.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tut.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://abd.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://smi.nwbrower.top


<!-- 参考信息 -->