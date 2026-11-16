代发 wailian999

Py:   len(arr)
来源：http://drj.gaohongyu789.top

PHP:  count($arr);
来源：http://tza.zhengqikj.top

JS:   arr.length
来源：http://cdc.epnwcf.com

TS:   arr.length
来源：http://osm.cucudq.cn

Java: list.size();
来源：http://glf.nanxinkj.top

Go:   len(arr)
来源：http://mvp.yj202588.top

Ruby: arr.length; arr.size
来源：http://rff.shzxlz.cn

C#:   list.Count;
来源：http://vnu.yvedp.cn

[D07] 切片 / 取子数组
来源：http://avl.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rfa.ctjpmb.com

PHP:  array_slice($arr, 1, 3);
来源：http://muj.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://wjo.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://wiz.aibaodan.cn

Java: list.subList(1, 4);
来源：http://hll.jinqigfzy.top

Go:   arr[1:4]
来源：http://dzx.cheryme.top

Ruby: arr[1, 3]
来源：http://wbx.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://rln.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://nzj.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://oxm.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://kbs.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://sab.fehbvm.com

TS:   [...a, ...b];
来源：http://abl.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lrq.cqqwz.cn

Go:   append(a, b...)
来源：http://upz.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://war.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://pvo.zhixingplan.top

[D09] 排序（升序）
来源：http://kby.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://fbe.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://yul.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wjt.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dpd.jqgfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lih.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nix.feifeiyinyue.top

Ruby: arr.sort
来源：http://tea.iojbl.cn

C#:   list.Sort();
来源：http://vml.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://evn.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://erm.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aga.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gmh.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyb.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kqh.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hrj.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ebk.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rnc.smart0.xyz

[D11] 反转数组
来源：http://mlc.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://hcu.zdbjq.cn

PHP:  array_reverse($arr);
来源：http://kgz.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://itf.gotoacloud.top

TS:   [...arr].reverse();
来源：http://sjt.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://qcl.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://osq.feifeiyinyue.top

Ruby: arr.reverse
来源：http://eui.andypj.xyz

C#:   list.Reverse();
来源：http://lmk.0kj1m.cn

[D12] 查找元素下标
来源：http://clv.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://buv.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bjx.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://czz.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://biu.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://meu.yj202588.top

Go:   slices.Index(arr, x)
来源：http://pzt.hcnkem.com

Ruby: arr.index(x)
来源：http://tjm.ybcxt.top

C#:   list.IndexOf(x);
来源：http://bqd.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://fvl.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dlk.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kkc.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://xtd.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://yho.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dtr.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ufi.zhiwuduotai.top

Ruby: arr.select { |x| x > 3 }
来源：http://vou.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nsx.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://zub.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gdt.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fvq.sweek.top

JS:   arr.map(x => x * 2)
来源：http://rsj.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://ktw.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bwb.shzxlz.cn

Go:   // 手写循环
来源：http://ceq.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xca.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uok.cucudq.cn

[D15] 去重
来源：http://lcx.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://clq.daria6918.cn

PHP:  array_unique($arr);
来源：http://yxf.uphjek.com

JS:   [...new Set(arr)]
来源：http://gpc.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://phl.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yml.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://icv.daxiang520.top

Ruby: arr.uniq
来源：http://hff.cashguo.top

C#:   list.Distinct().ToList()
来源：http://rcc.cheryme.top

[D16] 求和与平均值
来源：http://wfo.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gnp.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gyz.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vou.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ykt.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sme.jyoumei.cn

Go:   // 手写循环累加
来源：http://jjd.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://evq.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://yii.daxiang520.top

[D17] 最大值与最小值
来源：http://vgw.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://xja.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://atx.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rqs.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://ruo.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ybj.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xdz.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://pcb.ivvv.top

C#:   list.Max();  list.Min()
来源：http://bhg.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://wij.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ijk.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://lxc.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wth.hnxiangtu.top

TS:   nested.flat();
来源：http://kqx.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://esv.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://pbp.chenjidiqi.icu

Ruby: nested.flatten
来源：http://llv.jianghu66.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://inh.hysaishi.cn

[D19] 按字段分组
来源：http://ouj.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://smy.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hri.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qby.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nll.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cqg.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://lai.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lef.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://slz.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://zrd.ydjk.org.cn

Py:   Counter(arr)
来源：http://rhk.andypj.xyz

PHP:  array_count_values($arr);
来源：http://psx.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://owu.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://roo.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bxt.gaohongyu789.top

Go:   // 手写 map[T]int
来源：http://rak.fzhhl.top

Ruby: arr.tally
来源：http://znr.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jqg.smart0.xyz

[D21] 判断是否包含某元素
来源：http://zsj.birdmap.top

Py:   x in arr
来源：http://phn.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://lst.yongpay.top

JS:   arr.includes(x)
来源：http://day.birdmap.top

TS:   arr.includes(x)
来源：http://znl.feifeiyinyue.top

Java: list.contains(x)
来源：http://juz.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://lid.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://vjr.ydzc1.top

C#:   list.Contains(x)
来源：http://wkd.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://uap.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jzt.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nkb.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gvi.zhengqikj.top

TS:   [...arr];
来源：http://eqz.yfazqb.com

Java: new ArrayList<>(list);
来源：http://wtm.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://qvp.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://wrh.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://tvb.snrcjt.cn

[D23] reduce 累积计算
来源：http://fml.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cna.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jbq.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mex.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wzx.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://asi.ybcxt.top

Go:   // 手写循环
来源：http://rpw.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vda.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iht.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://hok.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bwp.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://igw.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rnw.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ahp.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://roc.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vdy.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pyb.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mzb.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://fpr.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ixw.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ayl.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ies.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jwx.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ryq.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bqq.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ifn.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tyz.cashguo.top

[D26] 数组转字符串
来源：http://uef.smart0.xyz

Py:   ", ".join(map(str, arr))
来源：http://kbe.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://oam.c1oappe.top

JS:   arr.join(", ")
来源：http://xhu.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://dhp.havefunace.top

Java: String.join(", ", list)
来源：http://rci.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://tla.havefunace.top

Ruby: arr.join(", ")
来源：http://and.ppjwa.cn

C#:   string.Join(", ", list)
来源：http://hgr.yanxiufei.cn

================================================================================
来源：http://slg.tianlin.xyz

E. 字符串处理
来源：http://bbn.iojbl.cn

================================================================================
来源：http://ann.cheryme.top

[E01] 拼接字符串
来源：http://qrv.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://urh.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mqb.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ddp.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nbh.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vai.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zvx.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gek.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tir.tanke756.top

[E02] 重复字符串
来源：http://pfu.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://vwy.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://him.iojbl.cn

JS:   "ab".repeat(3)
来源：http://eem.andypj.xyz

TS:   "ab".repeat(3)
来源：http://rpo.jiagoushi.top

Java: "ab".repeat(3)
来源：http://kkx.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://ebd.yj202588.top

Ruby: "ab" * 3
来源：http://tcq.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gcg.shzxlz.cn

[E03] 截取子串
来源：http://omp.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tih.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lge.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vcw.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://kao.sxryk.cn

Java: s.substring(1, 4)
来源：http://vos.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lnl.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://xdt.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://wzg.chenlongwang.top

[E04] 查找子串位置
来源：http://ntv.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://qxu.fehbvm.com

PHP:  strpos($s, "x");
来源：http://gdl.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://euo.316326.xyz

TS:   s.indexOf("x")
来源：http://yfa.gzhubu.top

Java: s.indexOf("x")
来源：http://gwv.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://mrx.zhongyouzk.top

Ruby: s.index("x")
来源：http://bqr.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://faj.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://znu.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gsp.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oiv.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xff.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://qyq.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iwe.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fvq.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cns.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cxy.shangyingyoupin.top

[E06] 替换子串
来源：http://zql.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pso.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://ajt.zhengqikj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fae.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://jam.hammf.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pyu.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qij.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fii.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://bps.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://ram.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vun.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rio.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wvv.zhijiandao.cn

TS:   s.split(",")
来源：http://lsq.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://vut.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jur.tarul.cn

Ruby: s.split(",");  s.split
来源：http://nzr.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dkj.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://nsa.zhiwuduotai.top

Py:   ",".join(items)
来源：http://qit.nanxinkj.top

PHP:  implode(",", $items);
来源：http://qoq.svipenyu.cn

JS:   items.join(",")
来源：http://qys.guannengcc.top

TS:   items.join(",")
来源：http://qav.sjlbkw.cn

Java: String.join(",", items)
来源：http://yhs.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://drv.cqqwz.cn

Ruby: items.join(",")
来源：http://pae.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://uoa.xuanzx.com

[E09] 去除所有空白字符
来源：http://hkz.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qyn.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://enh.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://cak.cqqwz.cn

TS:   s.replace(/\s+/g, "")
来源：http://oxy.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://egl.jiagoushi.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kqt.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://lqc.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gol.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://qeu.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xpj.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qhm.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://spw.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://ava.sweek.top

Java: String.format("%03d", 7)
来源：http://owo.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://rbx.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://unt.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lxp.zhongyouzk.top

[E11] 反转字符串
来源：http://ivh.dashuyun.cn

Py:   s[::-1]
来源：http://jjj.zhiwuduotai.top

PHP:  strrev($s);
来源：http://xgj.snrcjt.cn

JS:   [...s].reverse().join("")
来源：http://hbs.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://jzw.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://msx.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gjp.yj20258.top

Ruby: s.reverse
来源：http://pxz.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://phl.havefunace.top

[E12] 统计某字符出现次数
来源：http://vnq.fanxiaobao.xyz

Py:   s.count("a")
来源：http://njm.cashguo.top

PHP:  substr_count($s, "a");
来源：http://eru.iojbl.cn

JS:   s.split("a").length - 1
来源：http://ohh.gzhubu.top

TS:   s.split("a").length - 1
来源：http://aaz.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zwr.meibo888.top

Go:   strings.Count(s, "a")
来源：http://aua.zdbjq.cn

Ruby: s.count("a")
来源：http://nek.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://ojb.tanke756.top

[E13] 逐字符遍历
来源：http://vaf.tarul.cn


<!-- 参考信息 -->