代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwn.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lvu.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jjm.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://roz.iojbl.cn

Ruby: arr.index(x)
来源：http://mql.jinqigfzy.top

C#:   list.IndexOf(x);
来源：http://wxm.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://aoa.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://szg.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://spk.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://zsg.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://cjc.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ave.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gnq.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://cmz.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mjh.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://czm.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ecr.xylfe.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ppf.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://wma.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://fdn.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kgm.yanxiufei.cn

Go:   // 手写循环
来源：http://hyh.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ogs.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zix.daria6918.cn

[D15] 去重
来源：http://fie.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zrv.yfazqb.com

PHP:  array_unique($arr);
来源：http://bvq.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://lss.hesvh.cn

TS:   [...new Set(arr)]
来源：http://ods.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ifv.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://tps.zhiwuduotai.top

Ruby: arr.uniq
来源：http://eyo.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://tao.tianlin.xyz

[D16] 求和与平均值
来源：http://hok.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zbd.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wan.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mcu.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdk.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nie.sjlbkw.cn

Go:   // 手写循环累加
来源：http://ztq.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ehb.yj20258.top

C#:   list.Sum();  list.Average()
来源：http://jfn.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://afg.yongpay.top

Py:   max(arr);  min(arr)
来源：http://che.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://lvq.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jhp.fzhhl.top

TS:   Math.max(...arr);
来源：http://jfn.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://sae.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://any.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://qqt.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://ccv.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://pvn.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gjh.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://cqi.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://flz.jianghu66.top

TS:   nested.flat();
来源：http://lic.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://klm.gotoacloud.top

Go:   // 手写双层循环
来源：http://jgv.bjfxy.top

Ruby: nested.flatten
来源：http://jmz.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tht.hesvh.cn

[D19] 按字段分组
来源：http://ojh.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lxk.yangfankeji.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qpu.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aqk.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kxy.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lzs.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://ocz.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sfu.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nvh.jinqigfzy.top

[D20] 统计每个元素出现次数
来源：http://akz.vehdjk.com

Py:   Counter(arr)
来源：http://gjs.hcnkem.com

PHP:  array_count_values($arr);
来源：http://ctl.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wxd.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://saw.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pxk.c1oappe.top

Go:   // 手写 map[T]int
来源：http://pwc.zdqjudy.top

Ruby: arr.tally
来源：http://xcd.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kxw.pycfn.com

[D21] 判断是否包含某元素
来源：http://bmj.jqgufenzy.top

Py:   x in arr
来源：http://rep.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://sqq.jlsjyb.cn

JS:   arr.includes(x)
来源：http://xne.jiagoushi.top

TS:   arr.includes(x)
来源：http://njj.yuanzhike.top

Java: list.contains(x)
来源：http://ldj.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://vul.chenlongwang.top

Ruby: arr.include?(x)
来源：http://qut.hfpthk.cn

C#:   list.Contains(x)
来源：http://jhi.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://vxn.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tux.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kba.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oeg.c1oappe.top

TS:   [...arr];
来源：http://qna.redwolf501.top

Java: new ArrayList<>(list);
来源：http://thl.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://lsk.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://ppk.zhiwuduotai.top

C#:   new List<int>(list);
来源：http://lpm.ydzc1.top

[D23] reduce 累积计算
来源：http://bfr.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://amp.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://odr.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ons.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqh.redwolf501.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://blk.zhoulong.xyz

Go:   // 手写循环
来源：http://xhg.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ylc.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://soz.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://zuu.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qhm.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cst.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yml.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sky.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nep.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ado.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qhm.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wyz.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://vao.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bet.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hvo.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mma.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rlc.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eii.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uru.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aft.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wfs.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://naa.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://jcv.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://xen.gogol.net.cn

JS:   arr.join(", ")
来源：http://lya.hywenlv.cn

TS:   arr.join(", ")
来源：http://nba.jqgufenzy.top

Java: String.join(", ", list)
来源：http://yhn.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://prb.xziqi.cn

Ruby: arr.join(", ")
来源：http://xlk.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://gfs.gaohongyu789.top

================================================================================
来源：http://pwj.hnxiangtu.top

E. 字符串处理
来源：http://est.snrcjt.cn

================================================================================
来源：http://vwl.ppjwa.cn

[E01] 拼接字符串
来源：http://tsi.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tum.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fzp.guowangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://klv.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gra.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vpl.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fyo.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oev.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://exd.fktsv.cn

[E02] 重复字符串
来源：http://aov.c1oappe.top

Py:   "ab" * 3
来源：http://jst.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://egk.xylfe.cn

JS:   "ab".repeat(3)
来源：http://mpg.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://mpo.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://zvu.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://bzw.xziqi.cn

Ruby: "ab" * 3
来源：http://cpe.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mtm.gaohongyu789.top

[E03] 截取子串
来源：http://gcy.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oxc.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nif.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pcp.epnwcf.com

TS:   s.slice(1, 4)
来源：http://gsv.wangdashe.top

Java: s.substring(1, 4)
来源：http://nxq.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vqe.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://wlo.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://jte.jqgfzy.top

[E04] 查找子串位置
来源：http://wjg.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://rke.fktsv.cn

PHP:  strpos($s, "x");
来源：http://wpx.yanxiufei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vie.redwolf501.top

TS:   s.indexOf("x")
来源：http://zvn.aibaodan.cn

Java: s.indexOf("x")
来源：http://xim.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://lfz.yj20258888.top

Ruby: s.index("x")
来源：http://mnt.nwbrower.top

C#:   s.IndexOf("x")
来源：http://vog.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nqf.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kij.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tvj.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zeq.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://gts.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bud.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tpu.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bhb.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lgr.xylfe.cn

[E06] 替换子串
来源：http://aio.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://znk.yfazqb.com

PHP:  str_replace("a", "b", $s);
来源：http://mtp.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://seu.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://lxj.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pfh.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wge.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zrl.shangyingyoupin.top

C#:   s.Replace("a", "b")
来源：http://bxe.yueranfly.top

[E07] 按分隔符拆分
来源：http://hjc.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://trp.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xps.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fkb.xziqi.cn

TS:   s.split(",")
来源：http://ush.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://nsr.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rlh.kuanghao11.cn

Ruby: s.split(",");  s.split
来源：http://gyd.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dlh.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://xgf.yj202588.top

Py:   ",".join(items)
来源：http://tuw.jinyuanbaomall.cn

PHP:  implode(",", $items);
来源：http://zqd.xinyue.icu

JS:   items.join(",")
来源：http://fkj.snrcjt.cn

TS:   items.join(",")
来源：http://udf.shangyingyoupin.top

Java: String.join(",", items)
来源：http://rgg.sweek.top

Go:   strings.Join(items, ",")
来源：http://ycj.jinqigufen.top

Ruby: items.join(",")
来源：http://dji.316326.xyz

C#:   string.Join(",", items)
来源：http://enh.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://azy.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eez.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gjg.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://vtc.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://ifl.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://eie.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eej.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://eof.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fhi.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://onr.yj202588.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rkv.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ptn.daxiang520.top

JS:   "7".padStart(3, "0")
来源：http://upj.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://eie.tian-w.cn

Java: String.format("%03d", 7)
来源：http://jmf.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gcr.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qxs.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qqk.ivvv.top

[E11] 反转字符串
来源：http://tlw.nanxinkj.top

Py:   s[::-1]
来源：http://ish.ctjpmb.com

PHP:  strrev($s);
来源：http://tlw.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://hic.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://zhv.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://you.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ibc.kuanghao11.cn

Ruby: s.reverse
来源：http://tqc.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xsc.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://lil.tian-w.cn

Py:   s.count("a")
来源：http://gkn.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://qpx.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://vkc.yueranfly.top

TS:   s.split("a").length - 1
来源：http://tkd.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zeg.aibaodan.cn

Go:   strings.Count(s, "a")
来源：http://qbm.xuanzx.com

Ruby: s.count("a")
来源：http://ewm.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://ufq.haohaochexian.top

[E13] 逐字符遍历
来源：http://mdh.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://mcg.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ycc.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://czv.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ewp.shuidangran.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mfs.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kgq.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lmn.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vwn.aizwys.cn

[E14] URL 编码与 Base64
来源：http://kdz.shuidangran.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rim.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bow.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ngg.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://twn.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://awz.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tgq.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lzm.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ihd.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://rhq.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://bud.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zek.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bpf.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rhi.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nfu.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kco.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hlr.dashuyun.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dij.shzxlz.cn

[E16] 数字千分位
来源：http://hql.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://snh.svipenyu.cn

PHP:  number_format(1234567);
来源：http://frs.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bgz.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://egp.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pcq.meibo888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://czl.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://byb.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://jmz.fehbvm.com

[E17] 首字母大写
来源：http://hqu.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ymk.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://znv.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ivd.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bsr.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yzy.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://unq.mhx1999.top

Ruby: s.capitalize
来源：http://mxg.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ivo.nanxuanxn.top

[E18] 模板占位符替换
来源：http://hwz.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pae.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uno.zdbjq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tyu.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ywi.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vrk.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ehe.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://frf.snrcjt.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://imb.pycfn.com

[E19] 多行文本按行拆分
来源：http://hqm.svipenyu.cn

Py:   s.splitlines()
来源：http://mgi.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sml.redwolf501.top


<!-- 参考信息 -->