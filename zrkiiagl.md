代发 wailian999

TS:   [...arr].reverse();
来源：http://sxk.cdnleiting.top

Java: Collections.reverse(list);
来源：http://mos.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://eod.xuanzx.com

Ruby: arr.reverse
来源：http://bsz.hywenlv.cn

C#:   list.Reverse();
来源：http://qzv.chenjidiqi.icu

[D12] 查找元素下标
来源：http://mso.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://xeu.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dkb.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wmm.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://umu.aizwys.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://unk.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://fbi.gzhubu.top

Ruby: arr.index(x)
来源：http://uvj.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://yke.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://efy.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qji.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gte.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://krv.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://nos.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yfl.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dtu.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xdd.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://kwc.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://dbn.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://svp.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jba.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://kdh.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://gzj.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ifj.gogol.net.cn

Go:   // 手写循环
来源：http://exk.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://syc.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://muo.cheryme.top

[D15] 去重
来源：http://ros.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sug.chenzaomai.com

PHP:  array_unique($arr);
来源：http://nqd.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://moa.yj20258888.top

TS:   [...new Set(arr)]
来源：http://bze.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zic.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://hmj.yongpay.top

Ruby: arr.uniq
来源：http://lqb.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://vuj.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://tnx.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lrk.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dbk.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fyw.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vzf.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rbs.ydjk.org.cn

Go:   // 手写循环累加
来源：http://ljn.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nri.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://nqf.xziqi.cn

[D17] 最大值与最小值
来源：http://vga.sweek.top

Py:   max(arr);  min(arr)
来源：http://bkq.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://wdd.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gdn.daxiang520.top

TS:   Math.max(...arr);
来源：http://fks.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yql.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://umb.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://uel.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://eer.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://bjt.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nbd.yj20258.top

PHP:  array_merge(...$nested);
来源：http://isq.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ubp.zhongyouzk.top

TS:   nested.flat();
来源：http://ulp.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ayh.fktsv.cn

Go:   // 手写双层循环
来源：http://rib.pengpengdd.cyou

Ruby: nested.flatten
来源：http://lii.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://usl.chenjidiqi.icu

[D19] 按字段分组
来源：http://arf.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://edi.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jmn.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tti.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jzk.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nil.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://qht.jinghuilouyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://moi.zhixingplan.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://evr.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://euf.jinqigfzy.top

Py:   Counter(arr)
来源：http://znx.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://xjs.bjfxy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://osp.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wzs.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://abe.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://ptr.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://uyg.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mya.yonumen.top

[D21] 判断是否包含某元素
来源：http://rgi.nanxinkj.top

Py:   x in arr
来源：http://ker.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://yiu.yueranfly.top

JS:   arr.includes(x)
来源：http://xzn.jinqigfzy.top

TS:   arr.includes(x)
来源：http://ney.nanxuanxn.top

Java: list.contains(x)
来源：http://adz.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://ysl.9152youxi.cn

Ruby: arr.include?(x)
来源：http://ogz.bjfxy.top

C#:   list.Contains(x)
来源：http://noh.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://ruk.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pyi.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pno.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ihg.0kj1m.cn

TS:   [...arr];
来源：http://cel.316326.xyz

Java: new ArrayList<>(list);
来源：http://ysh.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://bdm.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://djy.sxryk.cn

C#:   new List<int>(list);
来源：http://zmd.ivvv.top

[D23] reduce 累积计算
来源：http://afc.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tts.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://akh.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pcl.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bet.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cxj.hnqzz.top

Go:   // 手写循环
来源：http://qly.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://umc.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jzw.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://iwm.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rlc.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pgn.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iox.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yyb.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qqa.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qqp.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ber.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gvr.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://ths.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://igm.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://chn.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nrv.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yez.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qnq.ydjk.org.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qgm.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xry.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://suk.nwbrower.top

[D26] 数组转字符串
来源：http://hru.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://fob.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://lew.jyoumei.cn

JS:   arr.join(", ")
来源：http://izf.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://nmj.bjfxy.top

Java: String.join(", ", list)
来源：http://jfi.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://yzm.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://byj.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://rzz.redwolf501.top

================================================================================
来源：http://ypi.zhengqikj.top

E. 字符串处理
来源：http://htr.hnqzz.top

================================================================================
来源：http://rbp.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://exv.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://igy.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oel.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ovc.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bqk.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lls.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rzc.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sjk.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bcy.yanxiufei.cn

[E02] 重复字符串
来源：http://abd.shuidangran.top

Py:   "ab" * 3
来源：http://ohw.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://zrg.cucudq.cn

JS:   "ab".repeat(3)
来源：http://beo.zycfv.cn

TS:   "ab".repeat(3)
来源：http://gwz.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://wrr.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://onk.dashuyun.cn

Ruby: "ab" * 3
来源：http://pnx.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://veo.yj202588.top

[E03] 截取子串
来源：http://ilj.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://auh.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hao.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mtw.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://vys.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://pcr.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xtx.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://aex.birdmap.top

C#:   s.Substring(1, 3)
来源：http://dvn.andypj.xyz

[E04] 查找子串位置
来源：http://nlx.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://gqm.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://kks.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cvt.chenlongwang.top

TS:   s.indexOf("x")
来源：http://ple.hesvh.cn

Java: s.indexOf("x")
来源：http://gue.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://dfs.sysykeji.top

Ruby: s.index("x")
来源：http://mpy.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://urv.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nmb.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fep.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pgd.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jib.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://rao.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rsg.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kvz.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ysh.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ngb.vehdjk.com

[E06] 替换子串
来源：http://fpk.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nxe.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://cnx.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yqp.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://dfm.hongshengwenyu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rxl.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eth.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://okq.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://mnk.zhengqikj.top

[E07] 按分隔符拆分
来源：http://kwn.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sxt.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kwu.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ass.guowangkeji.top

TS:   s.split(",")
来源：http://ukx.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://yhc.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sgy.ivvv.top

Ruby: s.split(",");  s.split
来源：http://rud.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wiv.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://csh.fehbvm.com

Py:   ",".join(items)
来源：http://drd.tarul.cn

PHP:  implode(",", $items);
来源：http://vfe.hysaishi.cn

JS:   items.join(",")
来源：http://veg.zhoulong.xyz

TS:   items.join(",")
来源：http://uuh.xuanzx.com

Java: String.join(",", items)
来源：http://rrw.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://iqy.uphjek.com

Ruby: items.join(",")
来源：http://hdq.ivvv.top

C#:   string.Join(",", items)
来源：http://cvu.yonumen.top

[E09] 去除所有空白字符
来源：http://qnf.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ucn.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mgg.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://qye.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://jvi.cucudq.cn

Java: s.replaceAll("\\s+", "")
来源：http://oti.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://erm.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://imp.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hxh.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://rnn.jqgufenzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bmv.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eio.birdmap.top

JS:   "7".padStart(3, "0")
来源：http://abx.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://evb.hammf.cn

Java: String.format("%03d", 7)
来源：http://xqh.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nku.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hzb.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pfr.jianghu66.top

[E11] 反转字符串
来源：http://vuu.jianghu66.top

Py:   s[::-1]
来源：http://gmr.guannengcc.top

PHP:  strrev($s);
来源：http://jnt.tanke756.top

JS:   [...s].reverse().join("")
来源：http://ayu.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://pvq.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://gso.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tjs.ivvv.top

Ruby: s.reverse
来源：http://loy.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://acv.tarul.cn

[E12] 统计某字符出现次数
来源：http://wqp.shangyingyoupin.top

Py:   s.count("a")
来源：http://bmo.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://ylx.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://htm.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://die.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://smg.yj202588.top

Go:   strings.Count(s, "a")
来源：http://qgk.zhijiandao.cn

Ruby: s.count("a")
来源：http://kvw.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://dgo.sysykeji.top

[E13] 逐字符遍历
来源：http://lnj.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://hdz.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mze.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://zgn.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://miz.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://smz.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jbw.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tak.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nci.birdmap.top

[E14] URL 编码与 Base64
来源：http://qln.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zpm.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://azf.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://arv.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vth.quarkkingdee.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://klj.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mqr.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hfi.zhoulong.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xqb.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://piz.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tcn.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ndv.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cdn.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pup.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://opu.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uil.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ptz.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bgw.zhijiandao.cn

[E16] 数字千分位
来源：http://mxa.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://cwf.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://jvc.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zsa.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hwi.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ywb.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yia.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wqu.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://mtv.cheryme.top

[E17] 首字母大写
来源：http://xxp.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fsf.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ufb.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iqo.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jop.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://law.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tzl.pycfn.com

Ruby: s.capitalize
来源：http://han.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wzb.yvedp.cn

[E18] 模板占位符替换
来源：http://xur.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vvm.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tdf.dianchejie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wbg.yueranfly.top


<!-- 参考信息 -->