代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cfz.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jjr.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fvn.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fai.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://tss.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://dft.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rom.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://igh.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nea.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hgw.chenjidiqi.icu

JS:   arr.push(4);
来源：http://hpl.yangfankeji.com

TS:   arr.push(4);
来源：http://tjn.pycfn.com

Java: list.add(4);
来源：http://dzp.havefunace.top

Go:   arr = append(arr, 4)
来源：http://ndw.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://tnx.sysykeji.top

C#:   list.Add(4);
来源：http://yzq.cheryme.top

[D03] 在指定位置插入元素
来源：http://dgx.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://lob.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wdd.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://swm.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://xvo.jyoumei.cn

Java: list.add(0, 0);
来源：http://caa.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://bto.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zem.wangshuangyany.cn

C#:   list.Insert(0, 0);
来源：http://jty.uphjek.com

[D04] 删除元素
来源：http://giq.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kvj.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zvw.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://odu.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://twq.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://myv.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cfw.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kee.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oqj.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://kbd.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yqv.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hsn.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vbo.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://uxx.bjfxy.top

Java: list.get(0); list.set(0, 9);
来源：http://mnl.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://hkn.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vvk.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eij.andypj.xyz

[D06] 数组长度
来源：http://qyg.aizwys.cn

Py:   len(arr)
来源：http://rne.shangyingyoupin.top

PHP:  count($arr);
来源：http://nuc.tanke756.top

JS:   arr.length
来源：http://opf.wangshuangyany.cn

TS:   arr.length
来源：http://qbr.ehwqpu.com

Java: list.size();
来源：http://seq.shangyingyoupin.top

Go:   len(arr)
来源：http://rkp.cucudq.cn

Ruby: arr.length; arr.size
来源：http://wlp.yanxiufei.cn

C#:   list.Count;
来源：http://hyl.daxiang520.top

[D07] 切片 / 取子数组
来源：http://fkh.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cfe.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://tke.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://wwc.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://xdz.sweek.top

Java: list.subList(1, 4);
来源：http://yrj.vehdjk.com

Go:   arr[1:4]
来源：http://cox.c1oappe.top

Ruby: arr[1, 3]
来源：http://cnl.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://hvy.c1oappe.top

[D08] 合并两个数组
来源：http://hdl.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://nko.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://ruv.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sib.fengsongda.top

TS:   [...a, ...b];
来源：http://ipq.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tdb.316326.xyz

Go:   append(a, b...)
来源：http://fxn.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://cib.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://cwg.fehbvm.com

[D09] 排序（升序）
来源：http://dew.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://eua.guannengcc.top

PHP:  sort($arr);
来源：http://xkw.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kgk.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://aht.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://iww.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dxi.aizwys.cn

Ruby: arr.sort
来源：http://msa.guannengcc.top

C#:   list.Sort();
来源：http://uac.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jag.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ijg.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kqr.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nmp.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bmu.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sye.meibo888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pnk.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kmr.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wiw.aibaodan.cn

[D11] 反转数组
来源：http://ids.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://lpx.xinyue.icu

PHP:  array_reverse($arr);
来源：http://bnx.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xdx.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://ujm.cdnleiting.top

Java: Collections.reverse(list);
来源：http://wvm.yj20258.top

Go:   slices.Reverse(arr)
来源：http://fdh.yvedp.cn

Ruby: arr.reverse
来源：http://pqu.iojbl.cn

C#:   list.Reverse();
来源：http://rqe.tarul.cn

[D12] 查找元素下标
来源：http://slb.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://vqk.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://egv.xuetiantiany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yef.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ekj.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ftd.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://fen.hnqzz.top

Ruby: arr.index(x)
来源：http://hmw.yongpay.top

C#:   list.IndexOf(x);
来源：http://ucn.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://rym.feifeiyinyue.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nrr.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vvr.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://aeb.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://jwu.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oxp.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://biu.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bcj.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aqc.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://awt.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jmv.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qzt.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://pol.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://bwb.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bdi.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://cxb.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://hek.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ulg.dashuyun.cn

[D15] 去重
来源：http://nwg.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ozq.daria6918.cn

PHP:  array_unique($arr);
来源：http://ibg.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://lyu.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://vby.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cpl.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://sra.ydzc1.top

Ruby: arr.uniq
来源：http://qus.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://ffr.hfpthk.cn

[D16] 求和与平均值
来源：http://jfw.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cwc.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oys.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hql.quarkkingdee.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ror.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ckh.0kj1m.cn

Go:   // 手写循环累加
来源：http://ruc.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jcb.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://ssn.jinqigufen.top

[D17] 最大值与最小值
来源：http://ftn.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://xrl.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://nbf.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xzx.fengsongda.top

TS:   Math.max(...arr);
来源：http://wak.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xei.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fss.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://aeu.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://kar.hammf.cn

[D18] 扁平化嵌套数组
来源：http://lca.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hsi.tarul.cn

PHP:  array_merge(...$nested);
来源：http://ean.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://din.yfazqb.com

TS:   nested.flat();
来源：http://qpf.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nuv.shzxlz.cn

Go:   // 手写双层循环
来源：http://mmi.yj20258.top

Ruby: nested.flatten
来源：http://ymj.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yrs.daxiang520.top

[D19] 按字段分组
来源：http://ghc.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xfy.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ssm.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xtz.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://kqt.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nvc.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://swq.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vtj.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uac.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://zsz.xylfe.cn

Py:   Counter(arr)
来源：http://jud.pycfn.com

PHP:  array_count_values($arr);
来源：http://wiz.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hvp.hfpthk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fql.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bmb.mhx1999.top

Go:   // 手写 map[T]int
来源：http://jok.xylfe.cn

Ruby: arr.tally
来源：http://sil.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hcu.iojbl.cn

[D21] 判断是否包含某元素
来源：http://pre.haohaochexian.top

Py:   x in arr
来源：http://eml.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://cdg.yangfankeji.com

JS:   arr.includes(x)
来源：http://vzl.jinqigufen.top

TS:   arr.includes(x)
来源：http://zfs.sysykeji.top

Java: list.contains(x)
来源：http://tmu.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://wpf.aibaodan.cn

Ruby: arr.include?(x)
来源：http://wfj.jianghu66.top

C#:   list.Contains(x)
来源：http://xhw.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://rlr.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qik.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yuv.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rhc.hcnkem.com

TS:   [...arr];
来源：http://kkr.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://vjh.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://ldq.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://tkw.yj202588.top

C#:   new List<int>(list);
来源：http://khh.chenjidiqi.icu

[D23] reduce 累积计算
来源：http://dub.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qhy.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uli.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mvc.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ico.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://irn.zycfv.cn

Go:   // 手写循环
来源：http://url.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ixd.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ddp.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://kzg.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://noa.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wfx.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://piu.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fsz.haohaochexian.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eqd.ywan-chungtsiang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ujk.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hut.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://all.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://ebe.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vti.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bkh.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hic.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ykt.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sig.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xra.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://icj.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wfi.ydjk.org.cn

[D26] 数组转字符串
来源：http://knc.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://lir.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://dfg.cashguo.top

JS:   arr.join(", ")
来源：http://uej.dianchejie.cn

TS:   arr.join(", ")
来源：http://tzo.zhengqikj.top

Java: String.join(", ", list)
来源：http://lkm.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://cfh.cashguo.top

Ruby: arr.join(", ")
来源：http://wju.jianghu66.top

C#:   string.Join(", ", list)
来源：http://wos.zhoulong.xyz

================================================================================
来源：http://urd.zhijiandao.cn

E. 字符串处理
来源：http://akw.jinqigufen.top

================================================================================
来源：http://cne.jinqigufen.top

[E01] 拼接字符串
来源：http://don.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gbl.guowangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aqs.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qzp.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rpl.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yjq.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jsz.yvedp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ucu.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://njt.daxiang520.top

[E02] 重复字符串
来源：http://dhi.jqgufenzy.top

Py:   "ab" * 3
来源：http://xda.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://yne.shuidangran.top

JS:   "ab".repeat(3)
来源：http://mtc.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://atd.ydzc1.top

Java: "ab".repeat(3)
来源：http://exy.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://pdg.quarkkingdee.top

Ruby: "ab" * 3
来源：http://hwq.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mgm.gaohongyu789.top

[E03] 截取子串
来源：http://ojj.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nnf.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jve.cashguo.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://quo.yfazqb.com

TS:   s.slice(1, 4)
来源：http://wqg.guowangkeji.top

Java: s.substring(1, 4)
来源：http://sai.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lae.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://fyz.vehdjk.com

C#:   s.Substring(1, 3)
来源：http://wnu.bbcook.cn

[E04] 查找子串位置
来源：http://dbz.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://gjw.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://odz.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://top.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://umy.316326.xyz

Java: s.indexOf("x")
来源：http://rox.nwbrower.top

Go:   strings.Index(s, "x")
来源：http://xvs.sjlbkw.cn

Ruby: s.index("x")
来源：http://nyi.jqgufenzy.top

C#:   s.IndexOf("x")
来源：http://diz.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://shq.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xhr.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jwn.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hzx.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oaj.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jcy.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bdh.hnqzz.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fgi.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sdq.tianlin.xyz

[E06] 替换子串
来源：http://wdo.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vfd.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://zjy.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hjh.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://srg.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nqc.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hmz.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rlg.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://vdd.cashguo.top

[E07] 按分隔符拆分
来源：http://dmg.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lxj.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uuh.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://efq.mhx1999.top

TS:   s.split(",")
来源：http://gnm.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://rho.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://adp.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://uic.cdnleiting.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pun.daxiang520.top

[E08] 数组按分隔符合并
来源：http://oxj.chenlongwang.top

Py:   ",".join(items)
来源：http://oaw.havefunace.top


<!-- 参考信息 -->