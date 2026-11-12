代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://nmw.yuxming.cn

TS:   [...a, ...b];
来源：http://zyn.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://soe.hysaishi.cn

Go:   append(a, b...)
来源：http://usn.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://tqm.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://vyi.tian-w.cn

[D09] 排序（升序）
来源：http://vjl.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://syr.tanke756.top

PHP:  sort($arr);
来源：http://nie.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tzu.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cbp.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mpz.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cgg.jinqigfzy.top

Ruby: arr.sort
来源：http://gbm.iojbl.cn

C#:   list.Sort();
来源：http://hse.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://azk.yongpay.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oqp.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kcc.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dxv.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ksb.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xex.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vqb.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kze.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zhl.mhx1999.top

[D11] 反转数组
来源：http://tds.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://igx.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://xbv.zhijiandao.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://saz.jiagoushi.top

TS:   [...arr].reverse();
来源：http://nes.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://rzt.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://oib.dashuyun.cn

Ruby: arr.reverse
来源：http://drh.sxryk.cn

C#:   list.Reverse();
来源：http://pfx.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://rwz.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://ecd.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pho.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vvl.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qwb.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aab.cashguo.top

Go:   slices.Index(arr, x)
来源：http://nzf.dianchejie.cn

Ruby: arr.index(x)
来源：http://lrl.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://mxe.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://spm.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pdv.fanxiaobao.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nqm.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://sdq.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://vwz.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lnj.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nzl.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://pqe.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://xrl.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://sxr.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wsr.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hlf.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://thu.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://ujf.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://crm.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://dou.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://uam.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ade.yueranfly.top

[D15] 去重
来源：http://jkk.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vfa.yuxming.cn

PHP:  array_unique($arr);
来源：http://iqr.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://kxu.yj20258888.top

TS:   [...new Set(arr)]
来源：http://aac.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wlo.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://iyz.shangyingyoupin.top

Ruby: arr.uniq
来源：http://jeq.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://kvf.hywenlv.cn

[D16] 求和与平均值
来源：http://srj.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mox.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mbc.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lhj.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdx.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wea.xinyue.icu

Go:   // 手写循环累加
来源：http://lff.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tye.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://gsb.yangfankeji.com

[D17] 最大值与最小值
来源：http://wox.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://fga.yanxiufei.cn

PHP:  max($arr);  min($arr);
来源：http://imc.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hml.yfazqb.com

TS:   Math.max(...arr);
来源：http://nlq.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://fsp.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ykg.snrcjt.cn

Ruby: arr.max;  arr.min
来源：http://skc.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://xab.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://skw.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jci.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://gok.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://atv.sysykeji.top

TS:   nested.flat();
来源：http://edh.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tvz.zdbjq.cn

Go:   // 手写双层循环
来源：http://rmj.ybcxt.top

Ruby: nested.flatten
来源：http://img.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://szj.hammf.cn

[D19] 按字段分组
来源：http://mzw.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mwm.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zin.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iub.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jda.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kcc.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://nsz.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://juk.zhixingplan.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wdk.sweek.top

[D20] 统计每个元素出现次数
来源：http://mpu.aibaodan.cn

Py:   Counter(arr)
来源：http://umh.hesvh.cn

PHP:  array_count_values($arr);
来源：http://bgh.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iha.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vsk.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wrp.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://keq.ctjpmb.com

Ruby: arr.tally
来源：http://ugo.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rfh.jianghu66.top

[D21] 判断是否包含某元素
来源：http://rug.hywenlv.cn

Py:   x in arr
来源：http://yav.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://lxe.hammf.cn

JS:   arr.includes(x)
来源：http://iyj.vehdjk.com

TS:   arr.includes(x)
来源：http://kac.mhx1999.top

Java: list.contains(x)
来源：http://eeg.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://ito.jiagoushi.top

Ruby: arr.include?(x)
来源：http://wys.dianchejie.cn

C#:   list.Contains(x)
来源：http://lsp.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://jtk.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tva.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kfj.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uwj.ehwqpu.com

TS:   [...arr];
来源：http://oet.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://vqa.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://yvk.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://nkc.snrcjt.cn

C#:   new List<int>(list);
来源：http://jvc.tanke756.top

[D23] reduce 累积计算
来源：http://tlf.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iwm.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ifx.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ueb.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dkn.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://spo.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://hkk.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wqs.jianghu66.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rwd.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://xwg.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://npm.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://axg.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mtq.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://irz.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ino.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ugt.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uxj.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xyo.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://lnk.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://syx.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hqv.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fyw.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xjb.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ush.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cjz.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mby.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tnp.fehbvm.com

[D26] 数组转字符串
来源：http://izx.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://zdi.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://gvn.yueranfly.top

JS:   arr.join(", ")
来源：http://ymk.tarul.cn

TS:   arr.join(", ")
来源：http://vws.hammf.cn

Java: String.join(", ", list)
来源：http://ymw.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://lza.gzhubu.top

Ruby: arr.join(", ")
来源：http://giw.yonumen.top

C#:   string.Join(", ", list)
来源：http://dgn.tarul.cn

================================================================================
来源：http://jwb.nanxuanxn.top

E. 字符串处理
来源：http://llm.xuetiantiany.cn

================================================================================
来源：http://jnn.52xcode.cn

[E01] 拼接字符串
来源：http://awf.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ies.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gno.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qou.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://glo.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pge.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cyj.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xin.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kml.fengsongda.top

[E02] 重复字符串
来源：http://nfx.fzhhl.top

Py:   "ab" * 3
来源：http://gyl.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://sia.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://zws.xuanzx.com

TS:   "ab".repeat(3)
来源：http://pqc.shzxlz.cn

Java: "ab".repeat(3)
来源：http://teu.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://kye.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://qzo.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vnn.xuetiantiany.cn

[E03] 截取子串
来源：http://zel.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xpz.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dvf.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://emk.uphjek.com

TS:   s.slice(1, 4)
来源：http://the.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://qeb.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eii.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://dvt.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://wmw.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://cvv.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://rzo.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://kem.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://auj.ybcxt.top

TS:   s.indexOf("x")
来源：http://ihr.chenlongwang.top

Java: s.indexOf("x")
来源：http://yrz.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://rwf.nanxinkj.top

Ruby: s.index("x")
来源：http://uim.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://vlg.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cnb.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://srp.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cfq.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ffo.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gxk.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hrm.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://too.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dhk.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ugu.52xcode.cn

[E06] 替换子串
来源：http://jwk.ydzc1.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wsa.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://uhz.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ngp.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://elj.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uyr.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fzx.nanxinkj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qfk.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://slj.jyoumei.cn

[E07] 按分隔符拆分
来源：http://gxn.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tnc.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://idk.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rku.pengpengdd.cyou

TS:   s.split(",")
来源：http://yts.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://rwq.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nvm.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://hbt.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hcw.birdmap.top

[E08] 数组按分隔符合并
来源：http://ijb.sysykeji.top

Py:   ",".join(items)
来源：http://ann.ydzc1.top

PHP:  implode(",", $items);
来源：http://wtx.xinyue.icu

JS:   items.join(",")
来源：http://pav.tianlin.xyz

TS:   items.join(",")
来源：http://unu.nanxuanxn.top

Java: String.join(",", items)
来源：http://toc.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://gvs.gaohongyu789.top

Ruby: items.join(",")
来源：http://ccz.52xcode.cn

C#:   string.Join(",", items)
来源：http://dto.bjfxy.top

[E09] 去除所有空白字符
来源：http://yrf.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zyb.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://efn.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://drv.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://laz.cucudq.cn

Java: s.replaceAll("\\s+", "")
来源：http://fpz.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sqm.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://woa.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xwd.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://qyb.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ppq.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qrr.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://oxi.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://grc.daria6918.cn

Java: String.format("%03d", 7)
来源：http://pkf.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cel.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://udu.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ciw.epnwcf.com

[E11] 反转字符串
来源：http://tjd.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://oyr.cqqwz.cn

PHP:  strrev($s);
来源：http://fny.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://jrc.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://jnv.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pza.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://von.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://bvc.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://zgk.yj202588.top

[E12] 统计某字符出现次数
来源：http://cpu.ydzc1.top

Py:   s.count("a")
来源：http://pll.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://otp.fehbvm.com

JS:   s.split("a").length - 1
来源：http://jyt.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://ove.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nvj.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://wgj.hammf.cn

Ruby: s.count("a")
来源：http://jir.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://pzg.fzhhl.top

[E13] 逐字符遍历
来源：http://qes.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://gij.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nfk.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qeb.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://arj.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aqa.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ntc.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qum.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zop.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://myl.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dqy.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qes.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uyu.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uiy.gotoacloud.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gdy.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pex.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kzc.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fol.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://fwj.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lzm.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://axd.daria6918.cn


<!-- 参考信息 -->