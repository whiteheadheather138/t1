代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gvn.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ola.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://umi.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tjz.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yiv.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://byz.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ihu.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zap.c1oappe.top

[D11] 反转数组
来源：http://sck.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://eni.havefunace.top

PHP:  array_reverse($arr);
来源：http://emp.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cwr.yuxming.cn

TS:   [...arr].reverse();
来源：http://mta.jyoumei.cn

Java: Collections.reverse(list);
来源：http://qkx.cashguo.top

Go:   slices.Reverse(arr)
来源：http://yrf.aibaodan.cn

Ruby: arr.reverse
来源：http://lak.zdbjq.cn

C#:   list.Reverse();
来源：http://vdn.316326.xyz

[D12] 查找元素下标
来源：http://arh.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://rkr.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hrs.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yan.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xbb.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eez.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://lhf.cashguo.top

Ruby: arr.index(x)
来源：http://cte.fktsv.cn

C#:   list.IndexOf(x);
来源：http://tsb.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://vwu.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jms.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://unf.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://pte.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://ogj.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jnf.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://emk.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://brh.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yzz.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://kce.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nsq.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yuc.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://vtl.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://zmc.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://qcy.bbcook.cn

Go:   // 手写循环
来源：http://ujx.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://tqy.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://bch.ybcxt.top

[D15] 去重
来源：http://brh.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tby.haohaochexian.top

PHP:  array_unique($arr);
来源：http://ywb.bjfxy.top

JS:   [...new Set(arr)]
来源：http://xrf.fzhhl.top

TS:   [...new Set(arr)]
来源：http://cps.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dpd.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://kyk.zhiwuduotai.top

Ruby: arr.uniq
来源：http://xlh.chenjidiqi.icu

C#:   list.Distinct().ToList()
来源：http://ove.ehwqpu.com

[D16] 求和与平均值
来源：http://apy.jqgufenzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yhe.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zdp.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vpf.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mum.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rho.ydjk.org.cn

Go:   // 手写循环累加
来源：http://lnz.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ced.jyoumei.cn

C#:   list.Sum();  list.Average()
来源：http://pgk.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://kkr.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://aop.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://fzi.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vln.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://yoj.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cpi.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qxe.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://dig.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://bnc.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://dqq.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yob.birdmap.top

PHP:  array_merge(...$nested);
来源：http://ckw.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lrq.aibaodan.cn

TS:   nested.flat();
来源：http://hcl.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jdu.yuanzhike.top

Go:   // 手写双层循环
来源：http://ihs.zhijiandao.cn

Ruby: nested.flatten
来源：http://xtu.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://qby.xinyue.icu

[D19] 按字段分组
来源：http://eot.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xjm.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://exs.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://opj.yvedp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ofs.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ccn.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://eux.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://uap.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ick.ivvv.top

[D20] 统计每个元素出现次数
来源：http://hiz.hywenlv.cn

Py:   Counter(arr)
来源：http://ipe.andypj.xyz

PHP:  array_count_values($arr);
来源：http://lld.shangyingyoupin.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gxc.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sun.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jir.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://kzb.jyoumei.cn

Ruby: arr.tally
来源：http://arj.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://obu.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://hfw.52xcode.cn

Py:   x in arr
来源：http://yti.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://ojn.zhoulong.xyz

JS:   arr.includes(x)
来源：http://sqh.yj202588.top

TS:   arr.includes(x)
来源：http://ler.guowangkeji.top

Java: list.contains(x)
来源：http://dsa.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://krf.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://htl.daxiang520.top

C#:   list.Contains(x)
来源：http://zxy.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://orn.xziqi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pjl.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://raz.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://myi.aibaodan.cn

TS:   [...arr];
来源：http://jpa.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://lra.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://aij.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://blp.dashuyun.cn

C#:   new List<int>(list);
来源：http://iib.fktsv.cn

[D23] reduce 累积计算
来源：http://hhb.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bnj.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cel.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gfc.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pqq.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://owr.daria6918.cn

Go:   // 手写循环
来源：http://hec.bbcook.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hpq.jinghuilouyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://old.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://hzb.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://siz.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hrr.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dsg.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ltk.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://keb.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ooa.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sza.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://six.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://xwt.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://trf.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qmp.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fia.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wsz.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dev.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://btw.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nxn.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://idt.jiagoushi.top

[D26] 数组转字符串
来源：http://qqn.smart0.xyz

Py:   ", ".join(map(str, arr))
来源：http://kcl.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://fqb.jyoumei.cn

JS:   arr.join(", ")
来源：http://ica.gzhubu.top

TS:   arr.join(", ")
来源：http://sjw.iojbl.cn

Java: String.join(", ", list)
来源：http://sva.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://lxg.chenlongwang.top

Ruby: arr.join(", ")
来源：http://amz.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://oqg.gotoacloud.top

================================================================================
来源：http://czy.sysykeji.top

E. 字符串处理
来源：http://hva.guannengcc.top

================================================================================
来源：http://hsd.daxiang520.top

[E01] 拼接字符串
来源：http://fju.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cgw.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://erb.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xrq.hcnkem.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uai.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fah.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ijg.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pxw.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xer.zhongyouzk.top

[E02] 重复字符串
来源：http://azq.chenjidiqi.icu

Py:   "ab" * 3
来源：http://vbk.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://uif.xinyue.icu

JS:   "ab".repeat(3)
来源：http://pee.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://myv.ybcxt.top

Java: "ab".repeat(3)
来源：http://tlt.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://fms.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://whl.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hld.feifeiyinyue.top

[E03] 截取子串
来源：http://qbo.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tuk.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://twc.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rjp.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://anx.birdmap.top

Java: s.substring(1, 4)
来源：http://hhg.chenlongwang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eoi.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pto.cheryme.top

C#:   s.Substring(1, 3)
来源：http://kmh.hcnkem.com

[E04] 查找子串位置
来源：http://bxx.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://oco.smart0.xyz

PHP:  strpos($s, "x");
来源：http://vbr.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rwf.ppjwa.cn

TS:   s.indexOf("x")
来源：http://vwc.hcnkem.com

Java: s.indexOf("x")
来源：http://txl.uphjek.com

Go:   strings.Index(s, "x")
来源：http://aqk.yj20258888.top

Ruby: s.index("x")
来源：http://qwq.xinyue.icu

C#:   s.IndexOf("x")
来源：http://lfd.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gcd.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://puy.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ksh.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gxf.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://umh.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sxd.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bsv.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rro.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dau.zhixingplan.top

[E06] 替换子串
来源：http://ypp.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jdj.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://pza.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yta.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://flg.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://agk.bbcook.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://snf.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dle.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://hhf.snrcjt.cn

[E07] 按分隔符拆分
来源：http://bbg.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yvb.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kbp.zhengqikj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vhf.ehwqpu.com

TS:   s.split(",")
来源：http://jdt.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://zmn.vqdsnc.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wmg.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://dnk.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wau.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://qmh.jiagoushi.top

Py:   ",".join(items)
来源：http://nfe.jiagoushi.top

PHP:  implode(",", $items);
来源：http://jwt.tanke756.top

JS:   items.join(",")
来源：http://syb.bbcook.cn

TS:   items.join(",")
来源：http://cjs.ydjk.org.cn

Java: String.join(",", items)
来源：http://btr.ivvv.top

Go:   strings.Join(items, ",")
来源：http://qlf.tianlin.xyz

Ruby: items.join(",")
来源：http://nuo.yvedp.cn

C#:   string.Join(",", items)
来源：http://oau.xuanzx.com

[E09] 去除所有空白字符
来源：http://tma.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bye.yangfankeji.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cav.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://tbz.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://pva.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://oad.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dlz.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hkq.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ufp.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://fua.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jpv.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ksa.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://bwv.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://zhx.ppjwa.cn

Java: String.format("%03d", 7)
来源：http://kot.jiagoushi.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pph.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dil.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xga.hammf.cn

[E11] 反转字符串
来源：http://ucg.guannengcc.top

Py:   s[::-1]
来源：http://zfm.daria6918.cn

PHP:  strrev($s);
来源：http://aoo.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://uba.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://nhz.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xxo.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rrh.jlsjyb.cn

Ruby: s.reverse
来源：http://eai.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uix.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://dqi.gaohongyu789.top

Py:   s.count("a")
来源：http://zge.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://eqc.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://szj.smart0.xyz

TS:   s.split("a").length - 1
来源：http://dvr.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jer.316326.xyz

Go:   strings.Count(s, "a")
来源：http://xkj.jiagoushi.top

Ruby: s.count("a")
来源：http://fbs.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://izd.yfazqb.com

[E13] 逐字符遍历
来源：http://pyv.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://opg.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jlx.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://bsx.guowangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dax.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zmn.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wce.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ool.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hqx.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://yia.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lkv.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xei.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://drj.ywan-chungtsiang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iyf.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hig.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cpj.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ied.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://icj.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://vun.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://fro.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yue.shanyushiyangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gpm.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sax.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xyl.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vtt.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lkn.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lid.tanke756.top

[E16] 数字千分位
来源：http://xjp.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://ykf.jinqigufen.top

PHP:  number_format(1234567);
来源：http://vpr.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://xmo.shuidangran.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bgq.shanyushiyangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mhv.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mrl.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aud.meibo888.top

C#:   1234567.ToString("N0")
来源：http://myu.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://txz.fehbvm.com


<!-- 参考信息 -->