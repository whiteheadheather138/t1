代发 wailian999

Ruby: arr.index(x)
来源：http://wys.cucudq.cn

C#:   list.IndexOf(x);
来源：http://bep.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://uuc.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ify.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ycc.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://yvz.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://fnc.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xyy.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pcr.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://iud.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jdh.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://ccj.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fdm.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://olu.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://ais.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://avz.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ymc.chenlongwang.top

Go:   // 手写循环
来源：http://etk.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xtn.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bju.kuanghao11.cn

[D15] 去重
来源：http://wco.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rjp.daxiang520.top

PHP:  array_unique($arr);
来源：http://xgu.havefunace.top

JS:   [...new Set(arr)]
来源：http://bqv.sysykeji.top

TS:   [...new Set(arr)]
来源：http://bjh.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gew.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://dma.meibo888.top

Ruby: arr.uniq
来源：http://jze.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://biu.ydjk.org.cn

[D16] 求和与平均值
来源：http://mtw.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jbg.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ppx.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rms.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zra.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zgl.yongpay.top

Go:   // 手写循环累加
来源：http://air.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dyr.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://flb.iojbl.cn

[D17] 最大值与最小值
来源：http://gcl.redwolf501.top

Py:   max(arr);  min(arr)
来源：http://bbh.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://cqu.ivvv.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rec.ehwqpu.com

TS:   Math.max(...arr);
来源：http://fwu.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kqe.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wxf.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://far.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://ays.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://njf.sjlbkw.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ggv.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://pis.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://swn.andypj.xyz

TS:   nested.flat();
来源：http://yvy.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jps.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://ydb.jqgufenzy.top

Ruby: nested.flatten
来源：http://ttw.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zms.tian-w.cn

[D19] 按字段分组
来源：http://mjz.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xaq.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bxq.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mdb.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dxs.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jon.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://wuq.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ekj.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iwv.pycfn.com

[D20] 统计每个元素出现次数
来源：http://xte.9152youxi.cn

Py:   Counter(arr)
来源：http://hap.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://hpg.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wzn.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://shx.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bhw.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://jwc.ehwqpu.com

Ruby: arr.tally
来源：http://bfc.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ovd.yj20258.top

[D21] 判断是否包含某元素
来源：http://cqk.yfazqb.com

Py:   x in arr
来源：http://ckp.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://kwb.quarkkingdee.top

JS:   arr.includes(x)
来源：http://eim.sweek.top

TS:   arr.includes(x)
来源：http://vcz.yanxiufei.cn

Java: list.contains(x)
来源：http://dmn.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://viv.cdnleiting.top

Ruby: arr.include?(x)
来源：http://akh.ybcxt.top

C#:   list.Contains(x)
来源：http://fnq.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://kmj.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yxr.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nhb.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sjj.wangdashe.top

TS:   [...arr];
来源：http://mbj.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://yry.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gkj.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://lkj.jqgfzy.top

C#:   new List<int>(list);
来源：http://vpf.gotoacloud.top

[D23] reduce 累积计算
来源：http://zyh.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dgj.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vbx.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kno.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rij.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ouu.nwbrower.top

Go:   // 手写循环
来源：http://nwi.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bmm.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zle.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://izw.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dsi.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ixb.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qcy.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mnz.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tbn.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://osx.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pdy.ehwqpu.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hox.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://xhp.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mcg.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ukf.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qqh.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gxs.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://elq.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kcd.hesvh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nxr.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kix.vqdsnc.cn

[D26] 数组转字符串
来源：http://qmn.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://cyr.316326.xyz

PHP:  implode(", ", $arr);
来源：http://wql.jianghu66.top

JS:   arr.join(", ")
来源：http://dmq.fktsv.cn

TS:   arr.join(", ")
来源：http://xsc.aizwys.cn

Java: String.join(", ", list)
来源：http://fyd.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://dfn.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://ame.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://tcx.fanxiaobao.xyz

================================================================================
来源：http://ebm.nanxinkj.top

E. 字符串处理
来源：http://iir.tanke756.top

================================================================================
来源：http://syu.iojbl.cn

[E01] 拼接字符串
来源：http://bog.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://icn.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bmn.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wsy.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jic.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kfl.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rlp.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iib.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://idx.sxryk.cn

[E02] 重复字符串
来源：http://yjj.zhijiandao.cn

Py:   "ab" * 3
来源：http://fyj.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://xpg.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://rmv.hnqzz.top

TS:   "ab".repeat(3)
来源：http://yrw.cucudq.cn

Java: "ab".repeat(3)
来源：http://ygg.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://pwn.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://iqd.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wom.0kj1m.cn

[E03] 截取子串
来源：http://xut.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lye.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kaj.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rkn.andypj.xyz

TS:   s.slice(1, 4)
来源：http://nah.hfpthk.cn

Java: s.substring(1, 4)
来源：http://bam.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xtm.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://znz.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://iqz.c1oappe.top

[E04] 查找子串位置
来源：http://zji.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://opr.nwbrower.top

PHP:  strpos($s, "x");
来源：http://wss.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qca.wangdashe.top

TS:   s.indexOf("x")
来源：http://xvv.smart0.xyz

Java: s.indexOf("x")
来源：http://adi.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://hfj.quarkkingdee.top

Ruby: s.index("x")
来源：http://ndq.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://lyb.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rlm.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://suq.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xly.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uiv.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://aan.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cvr.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xlb.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jaj.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hse.gotoacloud.top

[E06] 替换子串
来源：http://pdv.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qmm.ydjk.org.cn

PHP:  str_replace("a", "b", $s);
来源：http://pri.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iko.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://bet.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qqg.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://adl.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fqq.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://obp.fehbvm.com

[E07] 按分隔符拆分
来源：http://byf.sweek.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uvc.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kna.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qoe.yanxiufei.cn

TS:   s.split(",")
来源：http://nxq.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://sfn.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bsi.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://kjt.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pwg.zycfv.cn

[E08] 数组按分隔符合并
来源：http://pgb.aibaodan.cn

Py:   ",".join(items)
来源：http://ogr.fktsv.cn

PHP:  implode(",", $items);
来源：http://ebi.tanke756.top

JS:   items.join(",")
来源：http://jow.zycfv.cn

TS:   items.join(",")
来源：http://lww.9152youxi.cn

Java: String.join(",", items)
来源：http://rrk.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://jhl.hfpthk.cn

Ruby: items.join(",")
来源：http://bvq.nwbrower.top

C#:   string.Join(",", items)
来源：http://yyk.zhengqikj.top

[E09] 去除所有空白字符
来源：http://isg.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ajj.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qiv.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://gyj.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://sqk.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://sep.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dly.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lwy.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zoa.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://xtt.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oof.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bzi.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://kkh.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://fwf.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://otv.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ipz.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qtr.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kru.yj202588.top

[E11] 反转字符串
来源：http://bjq.smart0.xyz

Py:   s[::-1]
来源：http://ibg.iojbl.cn

PHP:  strrev($s);
来源：http://fuz.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://heo.yonumen.top

TS:   [...s].reverse().join("")
来源：http://ebg.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vpd.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zsg.nanxuanxn.top

Ruby: s.reverse
来源：http://myx.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://qrz.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://neo.birdmap.top

Py:   s.count("a")
来源：http://jzs.sweek.top

PHP:  substr_count($s, "a");
来源：http://nrm.yj20258.top

JS:   s.split("a").length - 1
来源：http://rqr.xuanzx.com

TS:   s.split("a").length - 1
来源：http://jnt.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mlt.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://yii.zhoulong.xyz

Ruby: s.count("a")
来源：http://uez.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://gsl.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://lyn.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://ffr.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kft.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dbd.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xbo.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uyy.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://czc.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dcn.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uwm.guannengcc.top

[E14] URL 编码与 Base64
来源：http://pcm.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://siy.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rty.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hyq.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fug.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tgh.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lvo.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ynd.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vhu.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://vhv.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://rlz.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vvu.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vid.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yty.vehdjk.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vuo.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rnh.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fie.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sfa.xinyue.icu

[E16] 数字千分位
来源：http://zss.yuxming.cn

Py:   f"{1234567:,}"
来源：http://sjf.hammf.cn

PHP:  number_format(1234567);
来源：http://aew.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ncy.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://htf.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tuo.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ysl.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bdr.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://kup.gogol.net.cn

[E17] 首字母大写
来源：http://lyf.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mox.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zqu.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ypc.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wvf.cashguo.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uhr.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zkn.hesvh.cn

Ruby: s.capitalize
来源：http://kaq.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rvu.wangdashe.top

[E18] 模板占位符替换
来源：http://tty.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eyg.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qrv.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pnl.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aov.chenjidiqi.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lex.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eqy.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hsx.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jtc.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://jzg.chenlongwang.top

Py:   s.splitlines()
来源：http://sca.zhaomingkeji.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qsd.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://bfq.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://vsb.zhaomingkeji.xyz

Java: s.lines().toList()
来源：http://ael.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://wyn.xylfe.cn


<!-- 参考信息 -->