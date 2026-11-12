代发 wailian999

Java: list.add(4);
来源：http://sfq.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://xqj.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://ohq.uphjek.com

C#:   list.Add(4);
来源：http://vrp.yongpay.top

[D03] 在指定位置插入元素
来源：http://gub.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://dms.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ztx.nanxuanxn.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oyi.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://jet.kuanghao11.cn

Java: list.add(0, 0);
来源：http://edd.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aoa.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://psb.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://tbd.0kj1m.cn

[D04] 删除元素
来源：http://eqr.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://guo.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fii.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rzo.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://puw.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jfn.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vpu.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pmr.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wmb.nanxuanxn.top

[D05] 访问与修改元素
来源：http://neb.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://knt.gaohongyu789.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tte.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wsc.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://krj.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://uow.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://kxt.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pcl.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mgp.0kj1m.cn

[D06] 数组长度
来源：http://qyk.tanke756.top

Py:   len(arr)
来源：http://xxt.gogol.net.cn

PHP:  count($arr);
来源：http://uow.zhoulong.xyz

JS:   arr.length
来源：http://jjn.andypj.xyz

TS:   arr.length
来源：http://tom.bbcook.cn

Java: list.size();
来源：http://whb.shanyushiyangkeji.top

Go:   len(arr)
来源：http://ltq.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://tat.hysaishi.cn

C#:   list.Count;
来源：http://pnw.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://lzh.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ven.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://cky.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://sqs.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://ujr.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://pgd.hysaishi.cn

Go:   arr[1:4]
来源：http://fco.hnqzz.top

Ruby: arr[1, 3]
来源：http://bed.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://wvt.fengsongda.top

[D08] 合并两个数组
来源：http://ypc.c1oappe.top

Py:   a + b;  a.extend(b)
来源：http://xaw.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://pnb.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dul.zhongyouzk.top

TS:   [...a, ...b];
来源：http://zmy.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jxe.hnxiangtu.top

Go:   append(a, b...)
来源：http://jly.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://qdo.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://qfw.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://vmc.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://qll.zhixingplan.top

PHP:  sort($arr);
来源：http://nbv.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lze.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ywf.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fyl.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yjt.chenzaomai.com

Ruby: arr.sort
来源：http://xqt.meibo888.top

C#:   list.Sort();
来源：http://qda.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iap.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mqb.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://foz.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hke.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://srg.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hvq.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://geh.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mcb.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://euk.jiagoushi.top

[D11] 反转数组
来源：http://mer.jianghu66.top

Py:   arr[::-1];  arr.reverse()
来源：http://iis.pycfn.com

PHP:  array_reverse($arr);
来源：http://sjf.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lex.yvedp.cn

TS:   [...arr].reverse();
来源：http://fxr.yj202588.top

Java: Collections.reverse(list);
来源：http://nmz.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://wkv.daria6918.cn

Ruby: arr.reverse
来源：http://oql.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://shi.zhongyouzk.top

[D12] 查找元素下标
来源：http://hkj.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://wgj.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bdt.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xlk.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nrl.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dpm.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://skh.mhx1999.top

Ruby: arr.index(x)
来源：http://kxn.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://hqt.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://rop.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gan.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://typ.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://cxh.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://knj.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://csn.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hek.zhiwuduotai.top

Ruby: arr.select { |x| x > 3 }
来源：http://lsj.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zmv.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://mtc.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lei.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pjs.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://tki.yvedp.cn

TS:   arr.map(x => x * 2)
来源：http://hif.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jbi.sjlbkw.cn

Go:   // 手写循环
来源：http://emh.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://hcd.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cpd.yonumen.top

[D15] 去重
来源：http://fvt.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://olz.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://wnw.guannengcc.top

JS:   [...new Set(arr)]
来源：http://rhn.sufxvd.cn

TS:   [...new Set(arr)]
来源：http://uew.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ejy.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://obp.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://lgi.316326.xyz

C#:   list.Distinct().ToList()
来源：http://gjz.aibaodan.cn

[D16] 求和与平均值
来源：http://zsr.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://icb.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sqa.xuetiantiany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tla.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kjc.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ycz.nwbrower.top

Go:   // 手写循环累加
来源：http://feu.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ebd.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://kxc.yuxming.cn

[D17] 最大值与最小值
来源：http://maq.yonumen.top

Py:   max(arr);  min(arr)
来源：http://lah.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://zkg.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kyb.uphjek.com

TS:   Math.max(...arr);
来源：http://gbb.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rql.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fen.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://tml.pycfn.com

C#:   list.Max();  list.Min()
来源：http://gxo.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://zlc.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vtg.ctjpmb.com

PHP:  array_merge(...$nested);
来源：http://akq.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tcf.xuetiantiany.cn

TS:   nested.flat();
来源：http://cnj.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://owb.dashuyun.cn

Go:   // 手写双层循环
来源：http://zno.nanxuanxn.top

Ruby: nested.flatten
来源：http://jbz.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cia.hfpthk.cn

[D19] 按字段分组
来源：http://ylf.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ufz.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nsq.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ncc.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://omv.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://shj.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://ufr.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://spl.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://amv.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://kef.zhongyouzk.top

Py:   Counter(arr)
来源：http://kuu.cheryme.top

PHP:  array_count_values($arr);
来源：http://nlb.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ory.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ees.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wwt.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://uov.jinqigfzy.top

Ruby: arr.tally
来源：http://duo.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rca.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://eee.xziqi.cn

Py:   x in arr
来源：http://oou.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://sot.daxiang520.top

JS:   arr.includes(x)
来源：http://nhf.xziqi.cn

TS:   arr.includes(x)
来源：http://kjw.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://fgf.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://peh.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://muk.yanxiufei.cn

C#:   list.Contains(x)
来源：http://muv.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://bxy.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cnw.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aki.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vlh.chenlongwang.top

TS:   [...arr];
来源：http://jjg.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://ghh.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iqq.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://hhz.yuanzhike.top

C#:   new List<int>(list);
来源：http://xsf.andypj.xyz

[D23] reduce 累积计算
来源：http://khb.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qip.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kzi.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yvk.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rgr.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://eqn.birdmap.top

Go:   // 手写循环
来源：http://wdf.yj20258.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bwn.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fmo.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://bix.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uoq.jqgfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lsp.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zob.yvedp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mxn.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hbn.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pnm.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hqz.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ekp.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://jmt.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fkl.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ggg.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fpp.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uta.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uow.chenjidiqi.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mvp.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xmx.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vlp.ivvv.top

[D26] 数组转字符串
来源：http://zit.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://wul.hammf.cn

PHP:  implode(", ", $arr);
来源：http://pqi.hysaishi.cn

JS:   arr.join(", ")
来源：http://evm.zhengqikj.top

TS:   arr.join(", ")
来源：http://kjb.andypj.xyz

Java: String.join(", ", list)
来源：http://vbf.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://muh.guannengcc.top

Ruby: arr.join(", ")
来源：http://fpd.daxiang520.top

C#:   string.Join(", ", list)
来源：http://zaq.gaohongyu789.top

================================================================================
来源：http://ywj.gzhubu.top

E. 字符串处理
来源：http://fhc.vehdjk.com

================================================================================
来源：http://jhn.zhongyouzk.top

[E01] 拼接字符串
来源：http://jkn.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ebj.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wnk.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gjm.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uzf.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bwm.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://isd.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nhf.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tvs.52xcode.cn

[E02] 重复字符串
来源：http://qbu.dashuyun.cn

Py:   "ab" * 3
来源：http://gfk.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://sij.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://cjy.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://vgl.pycfn.com

Java: "ab".repeat(3)
来源：http://pkl.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://awz.hysaishi.cn

Ruby: "ab" * 3
来源：http://ujm.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ucz.guowangkeji.top

[E03] 截取子串
来源：http://equ.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lkd.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rtq.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ulx.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://viv.0kj1m.cn

Java: s.substring(1, 4)
来源：http://hyx.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rmj.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kbp.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://nfr.52xcode.cn

[E04] 查找子串位置
来源：http://fht.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://vpn.guannengcc.top

PHP:  strpos($s, "x");
来源：http://sks.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qob.fktsv.cn

TS:   s.indexOf("x")
来源：http://hri.ydzc1.top

Java: s.indexOf("x")
来源：http://rfh.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://hdi.iojbl.cn

Ruby: s.index("x")
来源：http://iyt.52xcode.cn

C#:   s.IndexOf("x")
来源：http://mtv.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ice.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://egz.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hiq.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hmc.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tal.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rdz.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lyr.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rya.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://acc.yonumen.top

[E06] 替换子串
来源：http://hsd.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://icx.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://kdf.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://flr.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://aco.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dxg.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sar.hywenlv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dit.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://xaf.bjfxy.top

[E07] 按分隔符拆分
来源：http://fhf.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nir.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wjs.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://mhu.epnwcf.com

TS:   s.split(",")
来源：http://nha.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://rae.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oji.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://zao.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rfs.guannengcc.top

[E08] 数组按分隔符合并
来源：http://zgi.hnxiangtu.top

Py:   ",".join(items)
来源：http://ufq.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://eyv.ivvv.top

JS:   items.join(",")
来源：http://ihh.smart0.xyz

TS:   items.join(",")
来源：http://dex.sufxvd.cn

Java: String.join(",", items)
来源：http://oor.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://hgo.bjfxy.top

Ruby: items.join(",")
来源：http://zev.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://knl.yj202588.top

[E09] 去除所有空白字符
来源：http://unm.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lhq.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uoq.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://ypt.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://daz.xziqi.cn


<!-- 参考信息 -->