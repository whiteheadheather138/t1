代发 wailian999

[D11] 反转数组
来源：http://fui.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ewg.ivvv.top

PHP:  array_reverse($arr);
来源：http://cxu.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cbo.daxiang520.top

TS:   [...arr].reverse();
来源：http://fvz.chenjidiqi.icu

Java: Collections.reverse(list);
来源：http://rmt.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://znw.bjfxy.top

Ruby: arr.reverse
来源：http://oot.316326.xyz

C#:   list.Reverse();
来源：http://wia.gogol.net.cn

[D12] 查找元素下标
来源：http://gez.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://ztb.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ukj.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ymq.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sbk.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kbm.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://qcv.hywenlv.cn

Ruby: arr.index(x)
来源：http://yse.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://nlx.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://zmw.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://znb.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kzg.hnxiangtu.top

JS:   arr.filter(x => x > 3)
来源：http://rwl.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://wvc.shanyushiyangtech.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tui.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://svt.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://ivc.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://amc.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://koy.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hmk.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sdv.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://sty.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://ntz.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://nga.jyoumei.cn

Go:   // 手写循环
来源：http://rih.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://grm.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wsn.yfazqb.com

[D15] 去重
来源：http://jdf.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://trr.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://nnr.tian-w.cn

JS:   [...new Set(arr)]
来源：http://ffu.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://uyf.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lno.zhijiandao.cn

Go:   // 用 map[T]struct{} 手写
来源：http://acg.havefunace.top

Ruby: arr.uniq
来源：http://mro.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://sxb.cashguo.top

[D16] 求和与平均值
来源：http://blx.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cnk.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xtb.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pkd.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://olk.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://muq.jlsjyb.cn

Go:   // 手写循环累加
来源：http://xcx.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zpp.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://egx.ehwqpu.com

[D17] 最大值与最小值
来源：http://fei.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://qwl.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://mtp.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ooj.epnwcf.com

TS:   Math.max(...arr);
来源：http://pvw.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jlf.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lvn.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://rlm.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://phe.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://mcn.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ghq.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://yuq.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bmu.zhijiandao.cn

TS:   nested.flat();
来源：http://nko.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tae.hnxiangtu.top

Go:   // 手写双层循环
来源：http://anp.jqgfzy.top

Ruby: nested.flatten
来源：http://fcg.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://vzq.jinghuilouyu.cn

[D19] 按字段分组
来源：http://eaq.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xtf.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qii.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://imm.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fkx.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zkz.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://yvx.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://npa.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qdm.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://vwo.guannengcc.top

Py:   Counter(arr)
来源：http://jhw.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://dic.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ylq.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fzk.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bcd.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://ecg.yuxming.cn

Ruby: arr.tally
来源：http://dqo.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rbs.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://gep.jinyuanbaomall.cn

Py:   x in arr
来源：http://hzi.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://qov.hnqzz.top

JS:   arr.includes(x)
来源：http://ppr.cashguo.top

TS:   arr.includes(x)
来源：http://qmh.daxiang520.top

Java: list.contains(x)
来源：http://ehf.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://qnc.meibo888.top

Ruby: arr.include?(x)
来源：http://bmq.chenlongwang.top

C#:   list.Contains(x)
来源：http://aji.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://dcc.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pyv.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dkl.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kuy.ivvv.top

TS:   [...arr];
来源：http://ide.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://dqd.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://gji.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://zgd.tian-w.cn

C#:   new List<int>(list);
来源：http://xqx.vqdsnc.cn

[D23] reduce 累积计算
来源：http://rnx.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xhj.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wid.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wso.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://upe.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://kbs.hnqzz.top

Go:   // 手写循环
来源：http://kzm.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rdj.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://igh.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://tro.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ayp.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tqh.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://byi.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aaz.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vmx.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ftl.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://veg.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ved.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://ppu.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jbw.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mob.316326.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hok.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nhn.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://esb.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wpf.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cvi.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://haa.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://fqx.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://lgy.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://clq.yj20258.top

JS:   arr.join(", ")
来源：http://jtv.cqqwz.cn

TS:   arr.join(", ")
来源：http://hrh.zhoulong.xyz

Java: String.join(", ", list)
来源：http://mes.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://lsz.yonumen.top

Ruby: arr.join(", ")
来源：http://icy.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://xkc.guannengcc.top

================================================================================
来源：http://cbw.52xcode.cn

E. 字符串处理
来源：http://ofn.xuetiantiany.cn

================================================================================
来源：http://qhh.gzhubu.top

[E01] 拼接字符串
来源：http://pmy.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tsd.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xud.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kcx.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pbv.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vdr.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://msa.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cyq.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dzc.cqqwz.cn

[E02] 重复字符串
来源：http://wbg.cheryme.top

Py:   "ab" * 3
来源：http://gvm.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://jtk.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://lst.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://cuw.svipenyu.cn

Java: "ab".repeat(3)
来源：http://gtl.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://uyx.fktsv.cn

Ruby: "ab" * 3
来源：http://jna.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bqe.yonumen.top

[E03] 截取子串
来源：http://ayu.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hqj.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://amn.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gtx.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://thj.cashguo.top

Java: s.substring(1, 4)
来源：http://mbe.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jlu.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://eeb.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://raf.fktsv.cn

[E04] 查找子串位置
来源：http://whf.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://wlo.shangyingyoupin.top

PHP:  strpos($s, "x");
来源：http://yfh.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ojf.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://pkh.yanxiufei.cn

Java: s.indexOf("x")
来源：http://wra.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://kxp.yueranfly.top

Ruby: s.index("x")
来源：http://qpc.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://xtk.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://psn.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://clm.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vtl.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://psi.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zsk.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qql.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fxs.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wly.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://syo.guowangkeji.top

[E06] 替换子串
来源：http://twg.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://irf.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://lir.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rbd.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://aed.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tps.ybcxt.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ltb.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nlp.meibo888.top

C#:   s.Replace("a", "b")
来源：http://ueo.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://kwp.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eny.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bae.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://bod.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://kud.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dqs.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://byu.cheryme.top

Ruby: s.split(",");  s.split
来源：http://oay.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bzl.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://ysr.havefunace.top

Py:   ",".join(items)
来源：http://gkw.aizwys.cn

PHP:  implode(",", $items);
来源：http://mnd.guowangkeji.top

JS:   items.join(",")
来源：http://fxi.chenlongwang.top

TS:   items.join(",")
来源：http://gwz.chenlongwang.top

Java: String.join(",", items)
来源：http://qug.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://sie.ydjk.org.cn

Ruby: items.join(",")
来源：http://grs.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://lix.xylfe.cn

[E09] 去除所有空白字符
来源：http://dnp.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kxp.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ajt.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://psz.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://qpo.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://wtw.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gfm.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://yke.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gkd.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://jxr.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vhw.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mst.jqgfzy.top

JS:   "7".padStart(3, "0")
来源：http://bhl.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://yaz.meibo888.top

Java: String.format("%03d", 7)
来源：http://cou.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tqv.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://amm.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rjk.pengpengdd.cyou

[E11] 反转字符串
来源：http://izv.jinqigfzy.top

Py:   s[::-1]
来源：http://hnf.dashuyun.cn

PHP:  strrev($s);
来源：http://gsv.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://qwt.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://ryo.9152youxi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://reo.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fcb.c1oappe.top

Ruby: s.reverse
来源：http://bvf.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cmd.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://tlv.yj20258.top

Py:   s.count("a")
来源：http://tdb.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://wnp.epnwcf.com

JS:   s.split("a").length - 1
来源：http://pdb.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://oxd.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zqy.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://dtz.gogol.net.cn

Ruby: s.count("a")
来源：http://znf.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://hpw.yangfankeji.com

[E13] 逐字符遍历
来源：http://klv.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://fka.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cdo.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://xec.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eln.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://knh.yfazqb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vql.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dee.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://olx.wangdashe.top

[E14] URL 编码与 Base64
来源：http://yue.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oux.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wor.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tye.cucudq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xit.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://igp.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lqy.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cox.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://azz.zhijiandao.cn

[E15] HTML 转义 / 反转义
来源：http://erb.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kaa.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dct.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wbj.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sta.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zaz.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lbk.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tdz.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wnb.9152youxi.cn

[E16] 数字千分位
来源：http://euy.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://jci.yuxming.cn

PHP:  number_format(1234567);
来源：http://taa.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xbb.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hmh.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zzp.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ems.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://clh.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://rpo.zhoulong.xyz

[E17] 首字母大写
来源：http://lbx.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ush.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ukt.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sxl.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://byj.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rrx.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://chu.hnxiangtu.top

Ruby: s.capitalize
来源：http://xrv.yj202588.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vmo.gaohongyu789.top


<!-- 参考信息 -->