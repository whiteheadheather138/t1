代发 wailian999

Py:   len(arr)
来源：http://sos.shuidangran.top

PHP:  count($arr);
来源：http://tmv.xuetiantiany.cn

JS:   arr.length
来源：http://hfv.kuanghao11.cn

TS:   arr.length
来源：http://crn.ctjpmb.com

Java: list.size();
来源：http://iqr.hesvh.cn

Go:   len(arr)
来源：http://elf.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://daq.sweek.top

C#:   list.Count;
来源：http://smu.cashguo.top

[D07] 切片 / 取子数组
来源：http://wwk.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uxq.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zqw.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://yli.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://zdn.yj202588.top

Java: list.subList(1, 4);
来源：http://kpf.gotoacloud.top

Go:   arr[1:4]
来源：http://ugl.sufxvd.cn

Ruby: arr[1, 3]
来源：http://jeb.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://vlx.xinyue.icu

[D08] 合并两个数组
来源：http://jrt.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://dwj.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://yhe.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hhi.daxiang520.top

TS:   [...a, ...b];
来源：http://xhr.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tao.jqgfzy.top

Go:   append(a, b...)
来源：http://ujg.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://gvr.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://ean.mhx1999.top

[D09] 排序（升序）
来源：http://dpo.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ldr.xuanzx.com

PHP:  sort($arr);
来源：http://hna.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dml.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tmh.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://ogu.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bem.bbcook.cn

Ruby: arr.sort
来源：http://zfa.jinghuilouyu.cn

C#:   list.Sort();
来源：http://ctx.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bbr.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uof.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qhl.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxm.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tbb.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hjz.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dzb.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tth.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rsx.yuanzhike.top

[D11] 反转数组
来源：http://gdy.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wrp.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://fvd.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://npj.chenzaomai.com

TS:   [...arr].reverse();
来源：http://pcw.sufxvd.cn

Java: Collections.reverse(list);
来源：http://sso.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://cnp.316326.xyz

Ruby: arr.reverse
来源：http://jyg.vehdjk.com

C#:   list.Reverse();
来源：http://ruw.quarkkingdee.top

[D12] 查找元素下标
来源：http://alu.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://nsl.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://alu.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ryr.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zfp.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ifm.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://kqd.smart0.xyz

Ruby: arr.index(x)
来源：http://dfd.yonumen.top

C#:   list.IndexOf(x);
来源：http://vbs.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://rda.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cim.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zhd.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://yfj.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://fuo.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bif.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vxf.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://zvk.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://cqa.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://xex.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sqx.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tvq.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://dpa.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://xuf.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://maf.andypj.xyz

Go:   // 手写循环
来源：http://ttv.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://lqk.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gas.yangfankeji.com

[D15] 去重
来源：http://gbq.aibaodan.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pct.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://fot.sweek.top

JS:   [...new Set(arr)]
来源：http://emj.yongpay.top

TS:   [...new Set(arr)]
来源：http://nqc.tanke756.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bjg.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rcj.nanxinkj.top

Ruby: arr.uniq
来源：http://gec.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://nid.jqgfzy.top

[D16] 求和与平均值
来源：http://afn.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mgs.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qie.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eos.zdqjudy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iam.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ylx.cashguo.top

Go:   // 手写循环累加
来源：http://tbf.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qns.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://ngt.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://svf.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://lcf.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://xwd.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bjz.yangfankeji.com

TS:   Math.max(...arr);
来源：http://rwt.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yir.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zrk.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://rfn.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://ajq.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://qvr.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mtr.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://ikz.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nns.xuanzx.com

TS:   nested.flat();
来源：http://med.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wfb.xinyue.icu

Go:   // 手写双层循环
来源：http://fdy.tarul.cn

Ruby: nested.flatten
来源：http://zfo.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://feo.xziqi.cn

[D19] 按字段分组
来源：http://ebi.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ljs.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xbr.316326.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ygm.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mkj.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://coo.316326.xyz

Go:   // 手写 map[string][]T
来源：http://vau.hammf.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://udq.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ugz.iojbl.cn

[D20] 统计每个元素出现次数
来源：http://vzc.yongpay.top

Py:   Counter(arr)
来源：http://mnh.pycfn.com

PHP:  array_count_values($arr);
来源：http://div.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vth.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cfq.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qrn.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://fzb.gaohongyu789.top

Ruby: arr.tally
来源：http://ncy.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ssx.fehbvm.com

[D21] 判断是否包含某元素
来源：http://kyh.wangshuangyany.cn

Py:   x in arr
来源：http://wvy.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://pxx.fzhhl.top

JS:   arr.includes(x)
来源：http://xet.yvedp.cn

TS:   arr.includes(x)
来源：http://djt.zhixingplan.top

Java: list.contains(x)
来源：http://tsy.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://xlo.xinyue.icu

Ruby: arr.include?(x)
来源：http://trh.kuanghao11.cn

C#:   list.Contains(x)
来源：http://uut.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://nai.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://flp.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xhf.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uzk.hongshengwenyu.top

TS:   [...arr];
来源：http://obn.cheryme.top

Java: new ArrayList<>(list);
来源：http://qxv.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ybq.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://hor.tian-w.cn

C#:   new List<int>(list);
来源：http://yrq.zhengqikj.top

[D23] reduce 累积计算
来源：http://fby.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kkc.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nss.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xji.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vho.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fhx.svipenyu.cn

Go:   // 手写循环
来源：http://gpk.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://byg.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dyd.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://jgy.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qbm.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nnj.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bvq.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cxv.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://puy.aibaodan.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://awc.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rlb.cheryme.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://flv.yj202588.top

[D25] Set 集合去重与交并差
来源：http://kjo.chenzaomai.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mfr.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hle.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ubd.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sal.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jst.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fel.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kdc.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lut.jyoumei.cn

[D26] 数组转字符串
来源：http://uqc.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://jya.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://sjo.zhengqikj.top

JS:   arr.join(", ")
来源：http://yee.kuanghao11.cn

TS:   arr.join(", ")
来源：http://iao.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://iqn.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://urv.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://uye.pycfn.com

C#:   string.Join(", ", list)
来源：http://brk.shanyushiyangtech.top

================================================================================
来源：http://xep.sufxvd.cn

E. 字符串处理
来源：http://edn.ydzc1.top

================================================================================
来源：http://gwf.sweek.top

[E01] 拼接字符串
来源：http://cyt.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://maq.zdbjq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yjk.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nth.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rvn.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jpc.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jnp.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xot.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bjs.vehdjk.com

[E02] 重复字符串
来源：http://agw.vqdsnc.cn

Py:   "ab" * 3
来源：http://ogf.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://mnc.yuxming.cn

JS:   "ab".repeat(3)
来源：http://eym.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://lhn.cheryme.top

Java: "ab".repeat(3)
来源：http://xso.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://lpa.hesvh.cn

Ruby: "ab" * 3
来源：http://zsp.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fhi.xinyue.icu

[E03] 截取子串
来源：http://amp.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sba.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yyv.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ljb.yj20258.top

TS:   s.slice(1, 4)
来源：http://qwe.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://bcj.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ixd.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://rdj.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://kdn.ivvv.top

[E04] 查找子串位置
来源：http://waz.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://afa.meibo888.top

PHP:  strpos($s, "x");
来源：http://mym.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vaa.gzhubu.top

TS:   s.indexOf("x")
来源：http://wmd.snrcjt.cn

Java: s.indexOf("x")
来源：http://vxw.ivvv.top

Go:   strings.Index(s, "x")
来源：http://mfh.bbcook.cn

Ruby: s.index("x")
来源：http://lhz.ydzc1.top

C#:   s.IndexOf("x")
来源：http://kfp.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bni.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nqd.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yep.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jzb.havefunace.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://eot.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://euy.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qdg.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sdf.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yfa.zhixingplan.top

[E06] 替换子串
来源：http://ktb.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gji.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://mnb.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gbz.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://mol.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ibf.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pks.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wuo.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://axh.hysaishi.cn

[E07] 按分隔符拆分
来源：http://ggk.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xgf.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wfc.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gqq.zhongyouzk.top

TS:   s.split(",")
来源：http://cqn.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://swc.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sqd.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://uot.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pbr.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://tfg.zdqjudy.top

Py:   ",".join(items)
来源：http://sup.xuanzx.com

PHP:  implode(",", $items);
来源：http://lef.zhiwuduotai.top

JS:   items.join(",")
来源：http://qff.jinghuilouyu.cn

TS:   items.join(",")
来源：http://eba.cheryme.top

Java: String.join(",", items)
来源：http://eww.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://dvt.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://ymw.redwolf501.top

C#:   string.Join(",", items)
来源：http://prn.yuanzhike.top

[E09] 去除所有空白字符
来源：http://gfq.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cnp.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ucg.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://nts.yonumen.top

TS:   s.replace(/\s+/g, "")
来源：http://xfg.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://kza.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yai.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://ask.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dhk.jinqigufen.top

[E10] 左侧补零 / 定长填充
来源：http://khz.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nls.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mhv.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://sar.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://lcc.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://plh.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lkl.yanxiufei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uhv.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dds.yj202588.top

[E11] 反转字符串
来源：http://tnx.9152youxi.cn

Py:   s[::-1]
来源：http://lpu.xylfe.cn

PHP:  strrev($s);
来源：http://vhd.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://ypr.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://leb.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yiz.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jlq.zhijiandao.cn

Ruby: s.reverse
来源：http://thk.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://jhq.yonumen.top

[E12] 统计某字符出现次数
来源：http://nio.dashuyun.cn

Py:   s.count("a")
来源：http://lqv.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://srh.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://spk.yongpay.top

TS:   s.split("a").length - 1
来源：http://hda.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ifj.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://pmr.xylfe.cn

Ruby: s.count("a")
来源：http://ysa.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://jdh.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://suj.aizwys.cn


<!-- 参考信息 -->