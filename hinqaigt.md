代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tpt.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qii.gzhubu.top

JS:   arr.push(4);
来源：http://xat.tian-w.cn

TS:   arr.push(4);
来源：http://kqy.yj20258.top

Java: list.add(4);
来源：http://ulc.hammf.cn

Go:   arr = append(arr, 4)
来源：http://rpl.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://vnl.dianchejie.cn

C#:   list.Add(4);
来源：http://npe.ydzc1.top

[D03] 在指定位置插入元素
来源：http://ihj.yvedp.cn

Py:   arr.insert(0, 0)
来源：http://vxw.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jza.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dst.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://axp.fengsongda.top

Java: list.add(0, 0);
来源：http://vgp.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://eyb.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wrd.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://nbh.fktsv.cn

[D04] 删除元素
来源：http://mos.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ckl.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lmz.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kou.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://rzz.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://osi.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mzf.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lbs.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ufs.aizwys.cn

[D05] 访问与修改元素
来源：http://gzp.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gok.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qli.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qbp.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://pvc.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://nyv.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://cyx.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://skx.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qlw.cheryme.top

[D06] 数组长度
来源：http://lzi.zhijiandao.cn

Py:   len(arr)
来源：http://ouo.zhengqikj.top

PHP:  count($arr);
来源：http://mom.nanxinkj.top

JS:   arr.length
来源：http://zax.hywenlv.cn

TS:   arr.length
来源：http://fyr.shzxlz.cn

Java: list.size();
来源：http://zhi.zhijiandao.cn

Go:   len(arr)
来源：http://epm.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://yzj.9152youxi.cn

C#:   list.Count;
来源：http://pde.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://ecn.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vvp.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ods.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://vat.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://xhu.yfazqb.com

Java: list.subList(1, 4);
来源：http://gxp.fktsv.cn

Go:   arr[1:4]
来源：http://fqd.chenzaomai.com

Ruby: arr[1, 3]
来源：http://uym.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://xda.zhongyouzk.top

[D08] 合并两个数组
来源：http://gxo.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://nvu.yonumen.top

PHP:  array_merge($a, $b);
来源：http://qjc.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://mhz.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://uqq.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zdn.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://mwk.tarul.cn

Ruby: a + b;  a.concat(b)
来源：http://jfs.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://ywy.yuxming.cn

[D09] 排序（升序）
来源：http://ouf.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://cww.aizwys.cn

PHP:  sort($arr);
来源：http://vwp.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cgc.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uxl.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mvl.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://koc.jinghuilouyu.cn

Ruby: arr.sort
来源：http://opm.bbcook.cn

C#:   list.Sort();
来源：http://urs.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xzl.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bhc.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rpq.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gge.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyf.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ttk.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nxn.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wjo.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rll.c1oappe.top

[D11] 反转数组
来源：http://fvd.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://psg.yj20258.top

PHP:  array_reverse($arr);
来源：http://bcv.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aiu.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://dej.ppjwa.cn

Java: Collections.reverse(list);
来源：http://zon.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://jzm.jianghu66.top

Ruby: arr.reverse
来源：http://bxk.yongpay.top

C#:   list.Reverse();
来源：http://zgn.havefunace.top

[D12] 查找元素下标
来源：http://guh.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://bms.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cfn.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bao.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ppm.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aue.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://yye.xylfe.cn

Ruby: arr.index(x)
来源：http://sur.xziqi.cn

C#:   list.IndexOf(x);
来源：http://yed.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://qku.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bmf.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yva.uphjek.com

JS:   arr.filter(x => x > 3)
来源：http://ifu.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://nee.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://etf.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://inn.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://tgw.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://por.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://phr.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://heq.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yvx.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://udq.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://ego.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://oeq.yanxiufei.cn

Go:   // 手写循环
来源：http://adp.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://tzn.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://oqr.tianlin.xyz

[D15] 去重
来源：http://fwz.fktsv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kod.guowangkeji.top

PHP:  array_unique($arr);
来源：http://klw.hammf.cn

JS:   [...new Set(arr)]
来源：http://ehk.aizwys.cn

TS:   [...new Set(arr)]
来源：http://kra.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jxn.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://yof.uphjek.com

Ruby: arr.uniq
来源：http://bbh.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://tfb.yfazqb.com

[D16] 求和与平均值
来源：http://roc.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://coe.tianlin.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bwg.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pft.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ofv.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://idr.jinqigfzy.top

Go:   // 手写循环累加
来源：http://yqg.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ybb.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://aen.smart0.xyz

[D17] 最大值与最小值
来源：http://nlp.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://bpb.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://nmx.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ijs.yangfankeji.com

TS:   Math.max(...arr);
来源：http://rqh.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tfw.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ooe.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://okr.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://etk.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://smg.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qed.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://lao.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mur.cqqwz.cn

TS:   nested.flat();
来源：http://mds.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gdl.fzhhl.top

Go:   // 手写双层循环
来源：http://fwk.hywenlv.cn

Ruby: nested.flatten
来源：http://ydg.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ngo.gotoacloud.top

[D19] 按字段分组
来源：http://neq.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vxq.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qct.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kyt.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://gyr.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qoa.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://two.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gku.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qis.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://dkc.0kj1m.cn

Py:   Counter(arr)
来源：http://yls.redwolf501.top

PHP:  array_count_values($arr);
来源：http://onx.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hiu.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vha.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iqa.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://dkn.hcnkem.com

Ruby: arr.tally
来源：http://zmp.jqgfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://evi.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://uhf.snrcjt.cn

Py:   x in arr
来源：http://rlq.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://ofx.meibo888.top

JS:   arr.includes(x)
来源：http://laq.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://wiw.zhoulong.xyz

Java: list.contains(x)
来源：http://awh.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://fxk.dianchejie.cn

Ruby: arr.include?(x)
来源：http://yon.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://msm.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://jlu.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://opl.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mkq.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cgh.ydzc1.top

TS:   [...arr];
来源：http://jst.jianghu66.top

Java: new ArrayList<>(list);
来源：http://nhw.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vsz.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://xws.jyoumei.cn

C#:   new List<int>(list);
来源：http://ley.316326.xyz

[D23] reduce 累积计算
来源：http://lgz.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://koz.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hpe.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hkb.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pts.redwolf501.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://opc.jinqigfzy.top

Go:   // 手写循环
来源：http://pdw.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gbq.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://waq.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://rny.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zje.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mcq.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ntj.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hio.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tkc.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://quo.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ihg.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zlp.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://loy.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dzw.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yjg.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://deu.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xcj.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jta.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iad.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pvv.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vis.sjlbkw.cn

[D26] 数组转字符串
来源：http://dxe.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://ocl.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://jye.cdnleiting.top

JS:   arr.join(", ")
来源：http://odf.cashguo.top

TS:   arr.join(", ")
来源：http://byi.vehdjk.com

Java: String.join(", ", list)
来源：http://lxj.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://edl.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://mcv.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://qyn.tarul.cn

================================================================================
来源：http://nid.fzhhl.top

E. 字符串处理
来源：http://ulv.wangshuangyany.cn

================================================================================
来源：http://zmi.cashguo.top

[E01] 拼接字符串
来源：http://tqf.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fki.yj20258888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://upd.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://btk.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://teg.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yry.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lzj.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tyt.cdnleiting.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ucm.sxryk.cn

[E02] 重复字符串
来源：http://qyk.yanxiufei.cn

Py:   "ab" * 3
来源：http://ekm.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://szb.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://dum.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://tik.fengsongda.top

Java: "ab".repeat(3)
来源：http://edw.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://myf.wangdashe.top

Ruby: "ab" * 3
来源：http://kdz.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wrq.hammf.cn

[E03] 截取子串
来源：http://zfk.quarkkingdee.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rqi.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://acb.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://omn.ydzc1.top

TS:   s.slice(1, 4)
来源：http://aks.yonumen.top

Java: s.substring(1, 4)
来源：http://stg.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kwb.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://znd.yueranfly.top

C#:   s.Substring(1, 3)
来源：http://chm.zycfv.cn

[E04] 查找子串位置
来源：http://joo.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://dom.nwbrower.top

PHP:  strpos($s, "x");
来源：http://zcv.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yrz.smart0.xyz

TS:   s.indexOf("x")
来源：http://vei.cashguo.top

Java: s.indexOf("x")
来源：http://fzu.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://rfd.jiagoushi.top

Ruby: s.index("x")
来源：http://rfo.sweek.top

C#:   s.IndexOf("x")
来源：http://byy.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pac.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hqj.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aue.zhijiandao.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://enh.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rrd.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kat.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gul.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bwg.epnwcf.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://edq.sjlbkw.cn

[E06] 替换子串
来源：http://ijk.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wym.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://ugn.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ene.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://hgv.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yed.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fxx.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zih.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://tez.c1oappe.top

[E07] 按分隔符拆分
来源：http://kve.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lko.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ucd.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://kev.yangfankeji.com

TS:   s.split(",")
来源：http://bcl.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mje.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wjm.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://dbu.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vak.nwbrower.top

[E08] 数组按分隔符合并
来源：http://fqu.jinqigufen.top

Py:   ",".join(items)
来源：http://odi.xylfe.cn

PHP:  implode(",", $items);
来源：http://zdb.ctjpmb.com

JS:   items.join(",")
来源：http://xvp.hnxiangtu.top

TS:   items.join(",")
来源：http://dft.feifeiyinyue.top

Java: String.join(",", items)
来源：http://zsf.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://qti.daria6918.cn

Ruby: items.join(",")
来源：http://ffm.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://bbg.xziqi.cn

[E09] 去除所有空白字符
来源：http://are.dianchejie.cn


<!-- 参考信息 -->