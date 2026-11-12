代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bip.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://jix.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rop.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vme.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cge.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wkz.yangfankeji.com

[D05] 访问与修改元素
来源：http://itx.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oef.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fum.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yua.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://yru.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://xdr.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://zti.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vjt.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bjp.zdbjq.cn

[D06] 数组长度
来源：http://qcw.shzxlz.cn

Py:   len(arr)
来源：http://dbu.haohaochexian.top

PHP:  count($arr);
来源：http://lqy.pycfn.com

JS:   arr.length
来源：http://oeo.hfpthk.cn

TS:   arr.length
来源：http://bix.nwbrower.top

Java: list.size();
来源：http://ojw.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://jsr.aizwys.cn

Ruby: arr.length; arr.size
来源：http://fvk.meibo888.top

C#:   list.Count;
来源：http://cjj.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://yoo.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://woc.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://pqn.birdmap.top

JS:   arr.slice(1, 4);
来源：http://jha.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://dlz.ivvv.top

Java: list.subList(1, 4);
来源：http://jwm.haohaochexian.top

Go:   arr[1:4]
来源：http://zfw.gotoacloud.top

Ruby: arr[1, 3]
来源：http://ipl.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://qov.gogol.net.cn

[D08] 合并两个数组
来源：http://mku.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://gbu.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://xah.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aco.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://oxo.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kqq.shangyingyoupin.top

Go:   append(a, b...)
来源：http://dln.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://ctk.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://dol.xinyue.icu

[D09] 排序（升序）
来源：http://jrd.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://ggd.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://cxd.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jzj.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hth.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cpo.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nhp.uphjek.com

Ruby: arr.sort
来源：http://kgz.0kj1m.cn

C#:   list.Sort();
来源：http://gpg.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kmk.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zco.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yxl.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://odf.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ojb.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lbf.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rjv.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pfv.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gbb.ywan-chungtsiang.top

[D11] 反转数组
来源：http://bti.fzhhl.top

Py:   arr[::-1];  arr.reverse()
来源：http://joa.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://zit.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kak.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://dju.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://mle.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://vvp.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://agl.guowangkeji.top

C#:   list.Reverse();
来源：http://fqu.zycfv.cn

[D12] 查找元素下标
来源：http://lpw.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://ekn.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xvg.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fzf.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qap.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kpl.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://ijw.zdqjudy.top

Ruby: arr.index(x)
来源：http://qcs.cashguo.top

C#:   list.IndexOf(x);
来源：http://vtd.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://cmy.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uhv.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gck.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://btx.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://vae.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tbl.jqgfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rtb.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://shk.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://syr.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://udi.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mdj.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ymy.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://okf.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://rcv.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://lkv.mhx1999.top

Go:   // 手写循环
来源：http://gnf.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://icx.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dhc.xylfe.cn

[D15] 去重
来源：http://lkt.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://egh.daria6918.cn

PHP:  array_unique($arr);
来源：http://qne.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://omg.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://lql.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lrw.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sga.ydjk.org.cn

Ruby: arr.uniq
来源：http://hsv.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://cje.zhengqikj.top

[D16] 求和与平均值
来源：http://mrj.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zcx.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ljp.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oaw.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oom.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://glt.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://qgg.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://spp.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://cre.sxryk.cn

[D17] 最大值与最小值
来源：http://qmw.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://huu.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://vwj.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://omk.jiagoushi.top

TS:   Math.max(...arr);
来源：http://jvu.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ynr.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uwt.yongpay.top

Ruby: arr.max;  arr.min
来源：http://mzy.havefunace.top

C#:   list.Max();  list.Min()
来源：http://gkk.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://uxr.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uid.cheryme.top

PHP:  array_merge(...$nested);
来源：http://nek.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pym.feifeiyinyue.top

TS:   nested.flat();
来源：http://daj.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kuk.zhengqikj.top

Go:   // 手写双层循环
来源：http://xil.xziqi.cn

Ruby: nested.flatten
来源：http://yog.havefunace.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rjs.jianghu66.top

[D19] 按字段分组
来源：http://shm.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tew.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://whd.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ypb.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dht.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yyt.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://mnc.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jnl.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://diy.tarul.cn

[D20] 统计每个元素出现次数
来源：http://lyh.52xcode.cn

Py:   Counter(arr)
来源：http://cwq.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://pin.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nwh.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dwi.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tpy.gaohongyu789.top

Go:   // 手写 map[T]int
来源：http://qyv.hysaishi.cn

Ruby: arr.tally
来源：http://yis.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sly.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://hcq.yj202588.top

Py:   x in arr
来源：http://duq.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://yin.ppjwa.cn

JS:   arr.includes(x)
来源：http://fih.xylfe.cn

TS:   arr.includes(x)
来源：http://iqq.gogol.net.cn

Java: list.contains(x)
来源：http://efs.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://fks.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://lch.nanxinkj.top

C#:   list.Contains(x)
来源：http://ykz.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://leq.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ylb.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xvd.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kpe.ywan-chungtsiang.top

TS:   [...arr];
来源：http://yuk.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://aoy.zhaomingkeji.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://vvo.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://ref.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://fim.cucudq.cn

[D23] reduce 累积计算
来源：http://puc.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://snn.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jmy.cashguo.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://glx.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xvp.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://phl.hongshengwenyu.top

Go:   // 手写循环
来源：http://grr.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vya.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uwx.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://tqz.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wne.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://itl.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ssw.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ddm.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xth.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ccf.sjlbkw.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zrt.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gzq.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://fxw.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://erz.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jhr.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kzs.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://axb.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qmn.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://edm.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cvy.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://spx.hnqzz.top

[D26] 数组转字符串
来源：http://kjy.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://blc.meibo888.top

PHP:  implode(", ", $arr);
来源：http://qsr.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://bon.yonumen.top

TS:   arr.join(", ")
来源：http://emi.andypj.xyz

Java: String.join(", ", list)
来源：http://ixh.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://ffl.0kj1m.cn

Ruby: arr.join(", ")
来源：http://nzh.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://ber.fktsv.cn

================================================================================
来源：http://ccr.yonumen.top

E. 字符串处理
来源：http://xxp.tarul.cn

================================================================================
来源：http://adp.nanxinkj.top

[E01] 拼接字符串
来源：http://rwq.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kca.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cky.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://txx.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xrk.cashguo.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rch.yanxiufei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fsn.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wxi.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://brp.xuanzx.com

[E02] 重复字符串
来源：http://jwz.jqgfzy.top

Py:   "ab" * 3
来源：http://srb.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://dko.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://rep.yfazqb.com

TS:   "ab".repeat(3)
来源：http://dut.daria6918.cn

Java: "ab".repeat(3)
来源：http://qkh.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://ulf.kuanghao11.cn

Ruby: "ab" * 3
来源：http://abb.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bgu.cucudq.cn

[E03] 截取子串
来源：http://xfy.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wpg.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vgr.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://epy.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://dqr.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://zfc.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tsu.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ogl.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://lfr.hywenlv.cn

[E04] 查找子串位置
来源：http://tkf.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://gcy.epnwcf.com

PHP:  strpos($s, "x");
来源：http://tat.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://use.c1oappe.top

TS:   s.indexOf("x")
来源：http://afy.fengsongda.top

Java: s.indexOf("x")
来源：http://rim.cheryme.top

Go:   strings.Index(s, "x")
来源：http://fgh.fengsongda.top

Ruby: s.index("x")
来源：http://kgn.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://cym.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hms.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://beb.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vwm.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ttn.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://rmu.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ung.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nwl.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://urp.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://urf.gotoacloud.top

[E06] 替换子串
来源：http://iwe.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yqy.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://htv.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://auv.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://hvd.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://txo.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nfv.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bio.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://gqx.shzxlz.cn

[E07] 按分隔符拆分
来源：http://hsf.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yav.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zop.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ghv.zhoulong.xyz

TS:   s.split(",")
来源：http://wfw.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://dmu.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tdj.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://yxy.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lqk.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://nix.fehbvm.com

Py:   ",".join(items)
来源：http://vmk.iojbl.cn

PHP:  implode(",", $items);
来源：http://jem.redwolf501.top

JS:   items.join(",")
来源：http://tuy.chenzaomai.com

TS:   items.join(",")
来源：http://pac.svipenyu.cn

Java: String.join(",", items)
来源：http://vfk.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://qcv.sweek.top

Ruby: items.join(",")
来源：http://srf.sweek.top

C#:   string.Join(",", items)
来源：http://zhy.tanke756.top

[E09] 去除所有空白字符
来源：http://tou.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iph.snrcjt.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hzp.c1oappe.top

JS:   s.replace(/\s+/g, "")
来源：http://aps.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://poq.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://wop.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hep.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ill.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://esm.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://rcm.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ger.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://evn.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://svf.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://ybg.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://crz.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xtz.xziqi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://leu.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bkj.xziqi.cn

[E11] 反转字符串
来源：http://zvg.shuidangran.top

Py:   s[::-1]
来源：http://xtz.tianlin.xyz

PHP:  strrev($s);
来源：http://nay.shanyushiyangkeji.top


<!-- 参考信息 -->