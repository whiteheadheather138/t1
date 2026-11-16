代发 wailian999

C#:   list.Insert(0, 0);
来源：http://otz.vqdsnc.cn

[D04] 删除元素
来源：http://jbk.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vhk.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mkg.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pti.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://fiw.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bmb.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lgl.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mlp.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://frk.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://orf.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lpm.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wqx.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pqz.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://jzw.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://qad.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ifd.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://suz.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qyl.fktsv.cn

[D06] 数组长度
来源：http://abr.pycfn.com

Py:   len(arr)
来源：http://ghs.hysaishi.cn

PHP:  count($arr);
来源：http://ggw.shzxlz.cn

JS:   arr.length
来源：http://jck.quarkkingdee.top

TS:   arr.length
来源：http://yab.hnxiangtu.top

Java: list.size();
来源：http://nas.jqgufenzy.top

Go:   len(arr)
来源：http://bvi.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://qgs.tanke756.top

C#:   list.Count;
来源：http://siv.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://cvw.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fmw.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://vru.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://uax.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://mqi.yuanzhike.top

Java: list.subList(1, 4);
来源：http://fgd.chenjidiqi.icu

Go:   arr[1:4]
来源：http://eum.birdmap.top

Ruby: arr[1, 3]
来源：http://dba.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://jcq.tarul.cn

[D08] 合并两个数组
来源：http://xfy.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://pcy.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://qam.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jfq.52xcode.cn

TS:   [...a, ...b];
来源：http://vis.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zjz.andypj.xyz

Go:   append(a, b...)
来源：http://lxq.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://ltu.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://wck.cqqwz.cn

[D09] 排序（升序）
来源：http://yvr.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://kos.ppjwa.cn

PHP:  sort($arr);
来源：http://fvy.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xhf.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://xpp.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vqt.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vtg.meibo888.top

Ruby: arr.sort
来源：http://yzh.cqqwz.cn

C#:   list.Sort();
来源：http://omb.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xak.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qid.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tpm.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wyr.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qwt.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://svu.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rsu.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sqh.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lhy.ctjpmb.com

[D11] 反转数组
来源：http://jeu.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://byl.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://sal.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uef.ctjpmb.com

TS:   [...arr].reverse();
来源：http://tqb.xziqi.cn

Java: Collections.reverse(list);
来源：http://dvi.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://jcw.yvedp.cn

Ruby: arr.reverse
来源：http://dim.chenlongwang.top

C#:   list.Reverse();
来源：http://zek.yuanzhike.top

[D12] 查找元素下标
来源：http://yxp.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://cjz.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zlz.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sod.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://luu.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pqw.316326.xyz

Go:   slices.Index(arr, x)
来源：http://wsp.yvedp.cn

Ruby: arr.index(x)
来源：http://lvm.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://ufx.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://osk.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mef.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lnq.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://gla.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://zao.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hke.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gwe.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://var.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qup.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://ajo.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oxt.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ivs.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://mcl.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://iaf.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pla.hammf.cn

Go:   // 手写循环
来源：http://msq.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://jzo.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qab.chenlongwang.top

[D15] 去重
来源：http://owh.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ofa.0kj1m.cn

PHP:  array_unique($arr);
来源：http://xfh.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://iot.sweek.top

TS:   [...new Set(arr)]
来源：http://uev.zhijiandao.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://stn.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ciy.yvedp.cn

Ruby: arr.uniq
来源：http://ref.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://rqa.dianchejie.cn

[D16] 求和与平均值
来源：http://vsi.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kdb.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hnm.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jzj.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://afw.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jrd.hnqzz.top

Go:   // 手写循环累加
来源：http://jrk.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://llq.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://sqy.xuanzx.com

[D17] 最大值与最小值
来源：http://ubc.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://mjx.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://uvy.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uyc.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://sau.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ewb.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jkr.zhaomingkeji.xyz

Ruby: arr.max;  arr.min
来源：http://nsq.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://cbb.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://znz.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dwp.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://cmi.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tiy.tian-w.cn

TS:   nested.flat();
来源：http://nua.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kyw.aizwys.cn

Go:   // 手写双层循环
来源：http://zyn.cashguo.top

Ruby: nested.flatten
来源：http://dnz.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bja.shuidangran.top

[D19] 按字段分组
来源：http://tye.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://waj.wangdashe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vcd.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://srn.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kgk.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yvv.tarul.cn

Go:   // 手写 map[string][]T
来源：http://ihx.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jca.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://edl.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://ikd.pengpengdd.cyou

Py:   Counter(arr)
来源：http://qba.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://gzg.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fff.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jye.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dsp.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://zzj.guowangkeji.top

Ruby: arr.tally
来源：http://xth.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oip.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://nnf.hesvh.cn

Py:   x in arr
来源：http://nke.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://enq.yongpay.top

JS:   arr.includes(x)
来源：http://ugf.hysaishi.cn

TS:   arr.includes(x)
来源：http://sxh.smart0.xyz

Java: list.contains(x)
来源：http://ywg.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://krt.ppjwa.cn

Ruby: arr.include?(x)
来源：http://ytp.jiagoushi.top

C#:   list.Contains(x)
来源：http://byo.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://qxn.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lsv.chenjidiqi.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rjk.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zea.jianghu66.top

TS:   [...arr];
来源：http://qzj.cucudq.cn

Java: new ArrayList<>(list);
来源：http://mwl.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://fbf.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://srv.nanxinkj.top

C#:   new List<int>(list);
来源：http://plh.aizwys.cn

[D23] reduce 累积计算
来源：http://sgx.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yey.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zrt.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozy.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gxd.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cxz.9152youxi.cn

Go:   // 手写循环
来源：http://wfn.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fng.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ssi.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://yel.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xzt.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fmq.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://smt.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iyk.gaohongyu789.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mqr.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cwd.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zmt.gotoacloud.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tge.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://bbr.quarkkingdee.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mxi.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dpn.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://moa.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mde.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ygm.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xll.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rzk.nwbrower.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ico.haohaochexian.top

[D26] 数组转字符串
来源：http://kdt.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://epn.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://vkx.daria6918.cn

JS:   arr.join(", ")
来源：http://dxe.jianghu66.top

TS:   arr.join(", ")
来源：http://hss.c1oappe.top

Java: String.join(", ", list)
来源：http://eqb.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://zwy.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://sme.andypj.xyz

C#:   string.Join(", ", list)
来源：http://lvj.nanxinkj.top

================================================================================
来源：http://izw.fehbvm.com

E. 字符串处理
来源：http://yfk.c1oappe.top

================================================================================
来源：http://mpq.cucudq.cn

[E01] 拼接字符串
来源：http://wty.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://okj.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yfk.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ftk.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sqx.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://myq.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xla.sjlbkw.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rgd.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lyg.xziqi.cn

[E02] 重复字符串
来源：http://bbb.hywenlv.cn

Py:   "ab" * 3
来源：http://rqr.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://hoy.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://bid.wangdashe.top

TS:   "ab".repeat(3)
来源：http://dew.hysaishi.cn

Java: "ab".repeat(3)
来源：http://hpb.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://mvh.svipenyu.cn

Ruby: "ab" * 3
来源：http://eru.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uzx.sjlbkw.cn

[E03] 截取子串
来源：http://cwm.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://syi.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://omb.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cxq.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://fnj.hesvh.cn

Java: s.substring(1, 4)
来源：http://bww.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hnm.chenzaomai.com

Ruby: s[1, 3];  s[1..3]
来源：http://rpi.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://pqf.haohaochexian.top

[E04] 查找子串位置
来源：http://rnb.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://bhf.hcnkem.com

PHP:  strpos($s, "x");
来源：http://ecb.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jyk.smart0.xyz

TS:   s.indexOf("x")
来源：http://pby.gogol.net.cn

Java: s.indexOf("x")
来源：http://yfn.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://ind.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://keo.xuanzx.com

C#:   s.IndexOf("x")
来源：http://ekw.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sjz.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ppc.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mqr.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sos.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ljp.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bmv.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wlq.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ntl.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yvr.cheryme.top

[E06] 替换子串
来源：http://axx.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ckz.mhx1999.top

PHP:  str_replace("a", "b", $s);
来源：http://hov.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://njv.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://wcf.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tuo.yj20258888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xdy.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gum.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://xnp.cucudq.cn

[E07] 按分隔符拆分
来源：http://rjg.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kgu.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oeo.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zfy.0kj1m.cn

TS:   s.split(",")
来源：http://kwg.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://kjr.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://muv.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://xzb.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tqy.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://lrn.sxryk.cn

Py:   ",".join(items)
来源：http://ssc.tarul.cn

PHP:  implode(",", $items);
来源：http://dmj.jinghuilouyu.cn

JS:   items.join(",")
来源：http://uob.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://fws.cheryme.top

Java: String.join(",", items)
来源：http://ivd.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://sdp.bbcook.cn

Ruby: items.join(",")
来源：http://pnp.nanxuanxn.top

C#:   string.Join(",", items)
来源：http://uit.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://rhd.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oko.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://smq.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://mzx.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://kqg.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://zrw.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wjz.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://qzt.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uvt.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://kzc.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cbf.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wrt.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://ame.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://mho.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://iub.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vyh.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tst.dianchejie.cn


<!-- 参考信息 -->