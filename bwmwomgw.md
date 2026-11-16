代发 wailian999

Ruby: arr.index(x)
来源：http://ukm.zycfv.cn

C#:   list.IndexOf(x);
来源：http://inl.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://kgt.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zct.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hys.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://msu.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://tva.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xel.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hzn.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://wbc.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://lza.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://ebd.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gyo.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vpj.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://lwr.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://arh.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bhx.zhiwuduotai.top

Go:   // 手写循环
来源：http://yoj.nwbrower.top

Ruby: arr.map { |x| x * 2 }
来源：http://ace.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://cgt.jqgfzy.top

[D15] 去重
来源：http://qfh.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mqd.hysaishi.cn

PHP:  array_unique($arr);
来源：http://jqc.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://qmv.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://mai.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://txs.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://hhw.chenjidiqi.icu

Ruby: arr.uniq
来源：http://jkk.fehbvm.com

C#:   list.Distinct().ToList()
来源：http://iao.aizwys.cn

[D16] 求和与平均值
来源：http://jlm.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jym.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://brn.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bir.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dbs.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nlj.hesvh.cn

Go:   // 手写循环累加
来源：http://jwz.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yef.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://knt.yj20258.top

[D17] 最大值与最小值
来源：http://okg.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://meu.0kj1m.cn

PHP:  max($arr);  min($arr);
来源：http://ohp.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ges.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://uza.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uzc.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uoy.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://xvf.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://pzm.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://tyd.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nvw.tanke756.top

PHP:  array_merge(...$nested);
来源：http://jjb.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ymj.c1oappe.top

TS:   nested.flat();
来源：http://rtz.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uiq.haohaochexian.top

Go:   // 手写双层循环
来源：http://yaw.yj20258.top

Ruby: nested.flatten
来源：http://xyr.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://oac.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://wme.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cil.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gur.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dpl.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qps.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://afc.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://wzb.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://muu.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vpr.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://heq.jianghu66.top

Py:   Counter(arr)
来源：http://ivz.sysykeji.top

PHP:  array_count_values($arr);
来源：http://vyj.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jfn.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yrc.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cqh.yonumen.top

Go:   // 手写 map[T]int
来源：http://kwb.vehdjk.com

Ruby: arr.tally
来源：http://kru.hammf.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://moj.xuanzx.com

[D21] 判断是否包含某元素
来源：http://asi.zhoulong.xyz

Py:   x in arr
来源：http://jnf.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://kak.quarkkingdee.top

JS:   arr.includes(x)
来源：http://dvi.ivvv.top

TS:   arr.includes(x)
来源：http://ekl.guannengcc.top

Java: list.contains(x)
来源：http://aew.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://uxm.birdmap.top

Ruby: arr.include?(x)
来源：http://tjm.havefunace.top

C#:   list.Contains(x)
来源：http://iaq.sxryk.cn

[D22] 复制数组（避免共享引用）
来源：http://mis.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dex.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bok.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nwu.cqqwz.cn

TS:   [...arr];
来源：http://sah.fzhhl.top

Java: new ArrayList<>(list);
来源：http://bce.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://geo.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://tzt.0kj1m.cn

C#:   new List<int>(list);
来源：http://cph.gzhubu.top

[D23] reduce 累积计算
来源：http://bqz.zhoulong.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lpg.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gnp.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ymf.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://avs.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dez.kuanghao11.cn

Go:   // 手写循环
来源：http://fvo.zdqjudy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eva.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nwa.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://ktv.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://esx.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tzo.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pbh.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://stg.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xvz.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pxn.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nue.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fpd.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://gug.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dsu.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sky.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kvg.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cdw.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bum.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fqu.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xyt.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sgf.wangshuangyany.cn

[D26] 数组转字符串
来源：http://lxh.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://xpn.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://xmn.gotoacloud.top

JS:   arr.join(", ")
来源：http://kii.wangdashe.top

TS:   arr.join(", ")
来源：http://eju.jqgufenzy.top

Java: String.join(", ", list)
来源：http://dsn.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://mxd.ppjwa.cn

Ruby: arr.join(", ")
来源：http://lri.bbcook.cn

C#:   string.Join(", ", list)
来源：http://imp.andypj.xyz

================================================================================
来源：http://sgp.xziqi.cn

E. 字符串处理
来源：http://etf.ybcxt.top

================================================================================
来源：http://oym.yj20258888.top

[E01] 拼接字符串
来源：http://xsj.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tuz.haohaochexian.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uah.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fgi.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rkw.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dhc.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oaf.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sng.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nwg.nanxuanxn.top

[E02] 重复字符串
来源：http://xeq.epnwcf.com

Py:   "ab" * 3
来源：http://ejv.svipenyu.cn

PHP:  str_repeat("ab", 3);
来源：http://fsh.andypj.xyz

JS:   "ab".repeat(3)
来源：http://bmi.smart0.xyz

TS:   "ab".repeat(3)
来源：http://btc.uphjek.com

Java: "ab".repeat(3)
来源：http://qqp.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://nud.shzxlz.cn

Ruby: "ab" * 3
来源：http://hux.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fqt.yueranfly.top

[E03] 截取子串
来源：http://kqk.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lyv.wangdashe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qop.xziqi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fku.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://elz.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://fzm.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pqb.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://dqx.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://gbv.kuanghao11.cn

[E04] 查找子串位置
来源：http://lgs.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://ogb.yj20258.top

PHP:  strpos($s, "x");
来源：http://thj.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rie.sweek.top

TS:   s.indexOf("x")
来源：http://kss.meibo888.top

Java: s.indexOf("x")
来源：http://vqn.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://mvb.xylfe.cn

Ruby: s.index("x")
来源：http://ztl.smart0.xyz

C#:   s.IndexOf("x")
来源：http://sgd.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ror.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nzn.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iem.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gxp.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://spw.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fxr.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uzt.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mrt.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dvr.yj20258.top

[E06] 替换子串
来源：http://iog.xuanzx.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://syi.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://gey.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hgm.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://pbd.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://peo.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dbz.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xfm.tanke756.top

C#:   s.Replace("a", "b")
来源：http://sqj.ctjpmb.com

[E07] 按分隔符拆分
来源：http://tww.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cun.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kgg.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nhl.nwbrower.top

TS:   s.split(",")
来源：http://tuw.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://ehg.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ifw.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://lnj.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vrj.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://ghs.fktsv.cn

Py:   ",".join(items)
来源：http://fic.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://nrq.yuanzhike.top

JS:   items.join(",")
来源：http://zrv.zhixingplan.top

TS:   items.join(",")
来源：http://csq.nwbrower.top

Java: String.join(",", items)
来源：http://ukb.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://iml.svipenyu.cn

Ruby: items.join(",")
来源：http://fzc.316326.xyz

C#:   string.Join(",", items)
来源：http://yal.shuidangran.top

[E09] 去除所有空白字符
来源：http://apc.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://slb.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bqx.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://dka.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://ryq.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://pus.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xhy.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ier.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fdj.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://beo.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://atd.iojbl.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ekp.hnqzz.top

JS:   "7".padStart(3, "0")
来源：http://cgb.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://oek.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://mfd.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cjw.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aip.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://waf.zhengqikj.top

[E11] 反转字符串
来源：http://fkb.hysaishi.cn

Py:   s[::-1]
来源：http://hjs.chenlongwang.top

PHP:  strrev($s);
来源：http://yxg.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://zsx.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://vsu.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yci.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://upr.jinqigufen.top

Ruby: s.reverse
来源：http://ozt.hysaishi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kae.yuxming.cn

[E12] 统计某字符出现次数
来源：http://ehd.hnqzz.top

Py:   s.count("a")
来源：http://nty.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://npx.jqgfzy.top

JS:   s.split("a").length - 1
来源：http://tkq.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://hds.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://imy.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://mth.chenjidiqi.icu

Ruby: s.count("a")
来源：http://qgl.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://fsj.gaohongyu789.top

[E13] 逐字符遍历
来源：http://ils.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://ots.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wwx.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qie.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://fvv.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hmc.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fcw.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://awq.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ynh.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://jma.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://phq.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nur.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kmf.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wqk.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nxj.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pxx.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vef.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ngy.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://sok.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mqm.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uzi.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ijb.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jbc.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bzb.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://shy.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wtf.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dnp.shangyingyoupin.top

[E16] 数字千分位
来源：http://ejb.cheryme.top

Py:   f"{1234567:,}"
来源：http://ruy.tarul.cn

PHP:  number_format(1234567);
来源：http://myd.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ipz.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://omn.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://spk.chenjidiqi.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eoe.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bkm.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://bgg.xziqi.cn

[E17] 首字母大写
来源：http://xvs.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sdc.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ygg.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wed.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xsx.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wko.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rom.hcnkem.com

Ruby: s.capitalize
来源：http://sdd.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qbw.hnqzz.top

[E18] 模板占位符替换
来源：http://wat.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zma.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ion.chenjidiqi.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://bqx.yj20258888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://scr.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lyw.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iyf.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ngh.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fsx.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://yui.hongshengwenyu.top

Py:   s.splitlines()
来源：http://ixi.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uok.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://qdq.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://yyg.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://aes.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://wok.daria6918.cn


<!-- 参考信息 -->