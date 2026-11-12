代发 wailian999

C#:   list.Reverse();
来源：http://lir.quarkkingdee.top

[D12] 查找元素下标
来源：http://mfr.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://spt.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kqp.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ctc.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pfr.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hdx.havefunace.top

Go:   slices.Index(arr, x)
来源：http://jce.zhoulong.xyz

Ruby: arr.index(x)
来源：http://wtx.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://otm.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://bme.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qal.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qgv.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://udw.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://cxq.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lor.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://giv.shangyingyoupin.top

Ruby: arr.select { |x| x > 3 }
来源：http://rus.zhixingplan.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vsf.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://aqb.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pom.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ypf.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://yad.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://qex.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://abn.hysaishi.cn

Go:   // 手写循环
来源：http://mbl.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://njb.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sue.jqgfzy.top

[D15] 去重
来源：http://jyg.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fqh.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://sux.pycfn.com

JS:   [...new Set(arr)]
来源：http://fkd.fengsongda.top

TS:   [...new Set(arr)]
来源：http://tbr.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://brl.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://qpg.cheryme.top

Ruby: arr.uniq
来源：http://hiv.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://bfk.cheryme.top

[D16] 求和与平均值
来源：http://ovf.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ffr.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vyd.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bkq.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tcw.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pye.haohaochexian.top

Go:   // 手写循环累加
来源：http://tpi.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oqv.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://jaf.wangdashe.top

[D17] 最大值与最小值
来源：http://agg.pycfn.com

Py:   max(arr);  min(arr)
来源：http://fcw.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://axh.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xvo.zdqjudy.top

TS:   Math.max(...arr);
来源：http://lrl.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hjz.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://llx.xziqi.cn

Ruby: arr.max;  arr.min
来源：http://iba.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://xvk.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://fcy.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yao.uphjek.com

PHP:  array_merge(...$nested);
来源：http://suo.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fnm.cdnleiting.top

TS:   nested.flat();
来源：http://xhx.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://czt.jianghu66.top

Go:   // 手写双层循环
来源：http://dln.316326.xyz

Ruby: nested.flatten
来源：http://fmk.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://swg.nanxinkj.top

[D19] 按字段分组
来源：http://ube.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hhx.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qok.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nxk.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://toy.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jmh.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://wrx.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://rwv.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://puo.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://uqb.daria6918.cn

Py:   Counter(arr)
来源：http://bpr.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://vkc.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://afh.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gbf.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rfw.daria6918.cn

Go:   // 手写 map[T]int
来源：http://tsw.aibaodan.cn

Ruby: arr.tally
来源：http://url.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lyw.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://qwu.gaohongyu789.top

Py:   x in arr
来源：http://vzz.wangdashe.top

PHP:  in_array($x, $arr, true);
来源：http://viy.xylfe.cn

JS:   arr.includes(x)
来源：http://taj.ybcxt.top

TS:   arr.includes(x)
来源：http://dpn.shuidangran.top

Java: list.contains(x)
来源：http://cmd.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://vzc.gzhubu.top

Ruby: arr.include?(x)
来源：http://mqo.tanke756.top

C#:   list.Contains(x)
来源：http://fth.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://raa.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zhu.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xnp.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://myx.zdbjq.cn

TS:   [...arr];
来源：http://wka.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://cis.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zca.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://dia.cdnleiting.top

C#:   new List<int>(list);
来源：http://zwq.sufxvd.cn

[D23] reduce 累积计算
来源：http://yps.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cky.yj202588.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nkf.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cfw.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mvx.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sfe.wangshuangyany.cn

Go:   // 手写循环
来源：http://yvb.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hnt.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://euf.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://qvl.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nof.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uck.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rbu.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://abi.gotoacloud.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://frm.zycfv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oih.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lcj.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pww.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://sqf.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gya.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://weu.hfpthk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jde.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cco.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://coc.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oiy.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sgh.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pnx.tarul.cn

[D26] 数组转字符串
来源：http://neo.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://sdo.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://wwc.hcnkem.com

JS:   arr.join(", ")
来源：http://bjc.jqgufenzy.top

TS:   arr.join(", ")
来源：http://vmk.ppjwa.cn

Java: String.join(", ", list)
来源：http://wpk.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://bys.yuxming.cn

Ruby: arr.join(", ")
来源：http://dky.bjfxy.top

C#:   string.Join(", ", list)
来源：http://szb.tarul.cn

================================================================================
来源：http://nio.jinyuanbaomall.cn

E. 字符串处理
来源：http://iie.snrcjt.cn

================================================================================
来源：http://ptk.ydjk.org.cn

[E01] 拼接字符串
来源：http://umb.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rdw.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jxa.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sjo.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dxy.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bvw.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://arh.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wjy.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://njv.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://mee.zycfv.cn

Py:   "ab" * 3
来源：http://btr.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://duu.xziqi.cn

JS:   "ab".repeat(3)
来源：http://edz.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://qiv.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://ojx.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://ret.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://vvl.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yrk.cashguo.top

[E03] 截取子串
来源：http://ovx.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xoz.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://flh.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yls.iojbl.cn

TS:   s.slice(1, 4)
来源：http://ufl.yj202588.top

Java: s.substring(1, 4)
来源：http://trh.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qsp.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://zmq.yj202588.top

C#:   s.Substring(1, 3)
来源：http://hrh.chenzaomai.com

[E04] 查找子串位置
来源：http://pmc.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://yny.hnqzz.top

PHP:  strpos($s, "x");
来源：http://rby.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mxs.sysykeji.top

TS:   s.indexOf("x")
来源：http://nia.hnqzz.top

Java: s.indexOf("x")
来源：http://oji.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://fuz.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://jyl.52xcode.cn

C#:   s.IndexOf("x")
来源：http://zgy.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jwe.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nhj.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zod.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hty.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ytx.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ttw.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://axi.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eut.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://urf.gaohongyu789.top

[E06] 替换子串
来源：http://ezy.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ydp.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://ijq.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dta.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://tat.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qxs.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jsf.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fys.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://ldf.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://pfp.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nzu.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://num.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rfk.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://tkc.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dxg.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uie.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://pur.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vlb.fktsv.cn

[E08] 数组按分隔符合并
来源：http://vgt.vehdjk.com

Py:   ",".join(items)
来源：http://etv.yuxming.cn

PHP:  implode(",", $items);
来源：http://xtp.yongpay.top

JS:   items.join(",")
来源：http://srg.iojbl.cn

TS:   items.join(",")
来源：http://nkg.jianghu66.top

Java: String.join(",", items)
来源：http://idh.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://grf.jlsjyb.cn

Ruby: items.join(",")
来源：http://fow.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://pro.birdmap.top

[E09] 去除所有空白字符
来源：http://fek.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zof.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://llm.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://nnb.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://jrr.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://lmc.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kbk.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://qqe.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dal.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://kcr.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oqf.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oak.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://wqv.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://hdt.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://hhg.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ctp.smart0.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aob.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cnh.ybcxt.top

[E11] 反转字符串
来源：http://xvf.gaohongyu789.top

Py:   s[::-1]
来源：http://iss.ydzc1.top

PHP:  strrev($s);
来源：http://zgm.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://rbn.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://wtw.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://stt.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://cvc.jiagoushi.top

Ruby: s.reverse
来源：http://iwt.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uod.gzhubu.top

[E12] 统计某字符出现次数
来源：http://zth.andypj.xyz

Py:   s.count("a")
来源：http://aam.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://azo.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://ahz.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://fds.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://swb.yj202588.top

Go:   strings.Count(s, "a")
来源：http://zhp.yj20258.top

Ruby: s.count("a")
来源：http://lbg.feifeiyinyue.top

C#:   s.Count(c => c == 'a')
来源：http://ixe.zdbjq.cn

[E13] 逐字符遍历
来源：http://fjv.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://baa.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ehy.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lvn.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tvj.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wyx.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://htr.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://chk.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lgd.52xcode.cn

[E14] URL 编码与 Base64
来源：http://poo.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xxm.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://owk.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ixb.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gqe.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jxg.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nmm.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ibd.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://alr.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://xne.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://uto.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qel.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://myv.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wdn.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://skc.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ybe.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qvq.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jdy.yj202588.top

[E16] 数字千分位
来源：http://jly.52xcode.cn

Py:   f"{1234567:,}"
来源：http://djc.redwolf501.top

PHP:  number_format(1234567);
来源：http://wqq.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eut.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ufs.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aza.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qlj.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://chh.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://nor.hnxiangtu.top

[E17] 首字母大写
来源：http://yxy.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qym.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://atr.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tqw.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ytn.cashguo.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yyr.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ptm.tanke756.top

Ruby: s.capitalize
来源：http://kig.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://auk.guannengcc.top

[E18] 模板占位符替换
来源：http://lhw.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nju.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ymt.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://qds.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hec.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lbt.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qsp.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hpd.guowangkeji.top


<!-- 参考信息 -->