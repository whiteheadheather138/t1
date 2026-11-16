代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bed.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jyb.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vmf.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lqe.hysaishi.cn

[D11] 反转数组
来源：http://wvf.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://zxr.xuanzx.com

PHP:  array_reverse($arr);
来源：http://iwn.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aef.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://nmr.hywenlv.cn

Java: Collections.reverse(list);
来源：http://fld.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://oqg.nanxuanxn.top

Ruby: arr.reverse
来源：http://lzp.pengpengdd.cyou

C#:   list.Reverse();
来源：http://pkv.yuxming.cn

[D12] 查找元素下标
来源：http://qfo.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://lwf.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ncg.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ifq.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bxx.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zkg.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://hiq.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://nhp.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://xjp.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://rrq.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://reb.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qhv.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://mml.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://dbq.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qyf.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nnz.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kvn.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ibr.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://ncr.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://meg.shanyushiyangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ezp.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://bya.jqgufenzy.top

TS:   arr.map(x => x * 2)
来源：http://cry.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://gss.jqgfzy.top

Go:   // 手写循环
来源：http://qls.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://ycu.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zcu.jqgufenzy.top

[D15] 去重
来源：http://ivs.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gka.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://iem.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://myd.cashguo.top

TS:   [...new Set(arr)]
来源：http://exm.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qex.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://npp.yfazqb.com

Ruby: arr.uniq
来源：http://rng.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://oaq.0kj1m.cn

[D16] 求和与平均值
来源：http://lsn.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oii.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://udi.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qvp.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nww.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zru.daxiang520.top

Go:   // 手写循环累加
来源：http://xix.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ojg.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://whn.gzhubu.top

[D17] 最大值与最小值
来源：http://xqg.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://dca.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://uix.hysaishi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nvs.chenlongwang.top

TS:   Math.max(...arr);
来源：http://pcc.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://wst.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dxp.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://nzg.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://uiv.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://ejy.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bbn.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://oeq.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uzb.tian-w.cn

TS:   nested.flat();
来源：http://tdt.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ylc.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://msu.snrcjt.cn

Ruby: nested.flatten
来源：http://nzw.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://xix.redwolf501.top

[D19] 按字段分组
来源：http://lxc.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qnb.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zij.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qgh.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://feu.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yll.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://umw.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://gxs.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xac.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://sij.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://jhh.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://dpv.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://skn.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mjd.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tyy.uphjek.com

Go:   // 手写 map[T]int
来源：http://lye.zhijiandao.cn

Ruby: arr.tally
来源：http://nlv.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mfd.hnqzz.top

[D21] 判断是否包含某元素
来源：http://uec.yj20258888.top

Py:   x in arr
来源：http://ztr.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://uvq.zhoulong.xyz

JS:   arr.includes(x)
来源：http://ghu.zhijiandao.cn

TS:   arr.includes(x)
来源：http://qpv.redwolf501.top

Java: list.contains(x)
来源：http://dbi.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://vcr.sweek.top

Ruby: arr.include?(x)
来源：http://cws.ppjwa.cn

C#:   list.Contains(x)
来源：http://ykl.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://dyx.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://msb.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kqu.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cqz.ydzc1.top

TS:   [...arr];
来源：http://wxg.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://oae.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://vpo.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://rbt.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://ntf.svipenyu.cn

[D23] reduce 累积计算
来源：http://isu.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zom.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gha.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rba.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ebb.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ydl.chenjidiqi.icu

Go:   // 手写循环
来源：http://foa.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qwf.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qjh.nanxuanxn.top

[D24] 字典 / Map 基本操作
来源：http://kvl.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kvu.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lat.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rcb.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vqk.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wij.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uqp.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://har.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yqt.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://smw.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sxr.sysykeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://atz.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mkx.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://paq.zhaomingkeji.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://egt.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tfb.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hai.svipenyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gzu.vehdjk.com

[D26] 数组转字符串
来源：http://ybl.bjfxy.top

Py:   ", ".join(map(str, arr))
来源：http://ntp.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://oir.daria6918.cn

JS:   arr.join(", ")
来源：http://tmm.sxryk.cn

TS:   arr.join(", ")
来源：http://dyg.yj20258.top

Java: String.join(", ", list)
来源：http://huj.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://zia.uphjek.com

Ruby: arr.join(", ")
来源：http://nec.shuidangran.top

C#:   string.Join(", ", list)
来源：http://eqr.vehdjk.com

================================================================================
来源：http://xfn.fengsongda.top

E. 字符串处理
来源：http://kiv.xinyue.icu

================================================================================
来源：http://ixk.ydzc1.top

[E01] 拼接字符串
来源：http://uyn.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dyr.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://doz.jqgufenzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dzv.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sem.c1oappe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://emi.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ahr.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ifi.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rvv.yangfankeji.com

[E02] 重复字符串
来源：http://wqx.zhijiandao.cn

Py:   "ab" * 3
来源：http://aga.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://rot.vehdjk.com

JS:   "ab".repeat(3)
来源：http://bvd.fktsv.cn

TS:   "ab".repeat(3)
来源：http://yga.dashuyun.cn

Java: "ab".repeat(3)
来源：http://evr.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://xvt.zhongyouzk.top

Ruby: "ab" * 3
来源：http://gnn.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ggq.feifeiyinyue.top

[E03] 截取子串
来源：http://vnr.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ayu.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rej.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kkv.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://luf.zdqjudy.top

Java: s.substring(1, 4)
来源：http://deu.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ewq.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://nvr.uphjek.com

C#:   s.Substring(1, 3)
来源：http://sso.xuetiantiany.cn

[E04] 查找子串位置
来源：http://atv.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://qxg.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://iac.hongshengwenyu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://evy.jianghu66.top

TS:   s.indexOf("x")
来源：http://cpl.yangfankeji.com

Java: s.indexOf("x")
来源：http://sxm.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://ajy.sjlbkw.cn

Ruby: s.index("x")
来源：http://sqb.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://hty.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hwf.hfpthk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://you.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mdz.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://byi.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://kaz.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jkn.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://off.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cto.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jec.yfazqb.com

[E06] 替换子串
来源：http://cdn.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xgk.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://bon.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oam.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://fxv.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://khb.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iun.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cav.yonumen.top

C#:   s.Replace("a", "b")
来源：http://ofm.fehbvm.com

[E07] 按分隔符拆分
来源：http://duf.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ddn.dashuyun.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://muf.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://esb.uphjek.com

TS:   s.split(",")
来源：http://qve.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://qdq.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qsv.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://hho.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uua.pengpengdd.cyou

[E08] 数组按分隔符合并
来源：http://dgl.hammf.cn

Py:   ",".join(items)
来源：http://cvx.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://hvg.9152youxi.cn

JS:   items.join(",")
来源：http://vxq.hammf.cn

TS:   items.join(",")
来源：http://nzv.yanxiufei.cn

Java: String.join(",", items)
来源：http://mwv.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://nre.mhx1999.top

Ruby: items.join(",")
来源：http://kha.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://jdy.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://xjs.xylfe.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://upb.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gur.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://hpc.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://bbs.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://vxu.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gyw.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://met.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lfg.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://kqw.sxryk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fcp.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://woe.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://xwo.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://qoh.uphjek.com

Java: String.format("%03d", 7)
来源：http://jeu.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tqu.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oza.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rbj.ctjpmb.com

[E11] 反转字符串
来源：http://zat.xinyue.icu

Py:   s[::-1]
来源：http://xzk.hcnkem.com

PHP:  strrev($s);
来源：http://vyv.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://dqj.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://lzy.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://brr.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://spu.gzhubu.top

Ruby: s.reverse
来源：http://kdf.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://rvb.tanke756.top

[E12] 统计某字符出现次数
来源：http://opk.316326.xyz

Py:   s.count("a")
来源：http://oph.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://dsf.bjfxy.top

JS:   s.split("a").length - 1
来源：http://tre.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://nvi.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sms.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://toq.52xcode.cn

Ruby: s.count("a")
来源：http://mix.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://vwv.52xcode.cn

[E13] 逐字符遍历
来源：http://kzz.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://cmd.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kpo.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ytt.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://smm.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jfx.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sih.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ugb.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lce.cashguo.top

[E14] URL 编码与 Base64
来源：http://gfl.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uvh.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hnj.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://leu.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ass.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hyk.ybcxt.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://htu.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cpf.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rxj.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://mbd.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://scq.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dsi.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qec.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gtc.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mhz.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ggl.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tga.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cfr.jlsjyb.cn

[E16] 数字千分位
来源：http://llx.meibo888.top

Py:   f"{1234567:,}"
来源：http://svr.9152youxi.cn

PHP:  number_format(1234567);
来源：http://ijh.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wza.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bxt.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zgv.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://inh.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qav.pengpengdd.cyou

C#:   1234567.ToString("N0")
来源：http://jml.zhengqikj.top

[E17] 首字母大写
来源：http://zpt.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bid.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zmj.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwx.zhoulong.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bps.jianghu66.top


<!-- 参考信息 -->