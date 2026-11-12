代发 wailian999

C#:   list.Reverse();
来源：http://idk.daxiang520.top

[D12] 查找元素下标
来源：http://obp.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://cmx.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://izo.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fyi.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jib.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sub.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://bri.quarkkingdee.top

Ruby: arr.index(x)
来源：http://ozs.bjfxy.top

C#:   list.IndexOf(x);
来源：http://xxr.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://ltg.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vre.fktsv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bvy.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://jie.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://mnl.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jus.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bwb.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://bgo.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lqm.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://ygd.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gzw.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xme.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://shx.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://erd.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://okt.tianlin.xyz

Go:   // 手写循环
来源：http://oal.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dge.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qgh.kuanghao11.cn

[D15] 去重
来源：http://wsu.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jjb.chenzaomai.com

PHP:  array_unique($arr);
来源：http://for.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://llc.hnqzz.top

TS:   [...new Set(arr)]
来源：http://vcz.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uzc.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://uwj.chenzaomai.com

Ruby: arr.uniq
来源：http://cjs.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://sak.jinqigufen.top

[D16] 求和与平均值
来源：http://wvj.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hzi.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://obg.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rjr.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://otl.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uky.sufxvd.cn

Go:   // 手写循环累加
来源：http://qfe.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nrx.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://cmb.uphjek.com

[D17] 最大值与最小值
来源：http://npm.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://efu.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://dwi.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uzp.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://bhv.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rba.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gux.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://qfp.havefunace.top

C#:   list.Max();  list.Min()
来源：http://itm.bbcook.cn

[D18] 扁平化嵌套数组
来源：http://vyj.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zbw.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://qed.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://etn.andypj.xyz

TS:   nested.flat();
来源：http://rgy.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ium.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://baw.redwolf501.top

Ruby: nested.flatten
来源：http://lcm.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dei.jianghu66.top

[D19] 按字段分组
来源：http://kmg.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ksg.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ufu.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sfe.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://joo.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eem.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://gei.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rmi.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jdu.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://brq.wangdashe.top

Py:   Counter(arr)
来源：http://ruh.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://pfw.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://scn.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://woi.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sgb.daxiang520.top

Go:   // 手写 map[T]int
来源：http://atj.aibaodan.cn

Ruby: arr.tally
来源：http://khu.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hre.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://ukb.epnwcf.com

Py:   x in arr
来源：http://wcs.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://ddi.gzhubu.top

JS:   arr.includes(x)
来源：http://duw.fengsongda.top

TS:   arr.includes(x)
来源：http://rwp.jinqigufen.top

Java: list.contains(x)
来源：http://jrp.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://dcf.jiagoushi.top

Ruby: arr.include?(x)
来源：http://ies.yueranfly.top

C#:   list.Contains(x)
来源：http://uoa.jlsjyb.cn

[D22] 复制数组（避免共享引用）
来源：http://xyf.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vkh.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nvo.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://biu.fzhhl.top

TS:   [...arr];
来源：http://wad.sxryk.cn

Java: new ArrayList<>(list);
来源：http://swp.zhoulong.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://jge.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://iww.aizwys.cn

C#:   new List<int>(list);
来源：http://nrp.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://shi.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vpi.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qzl.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gnc.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zov.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://rjj.epnwcf.com

Go:   // 手写循环
来源：http://rth.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qcu.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jte.hnxiangtu.top

[D24] 字典 / Map 基本操作
来源：http://xos.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yyu.aizwys.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jfm.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ytu.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yuu.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://msj.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ixt.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://txf.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://odv.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://edx.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lkp.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qqm.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nda.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xly.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xun.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mkr.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://byc.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sqr.pycfn.com

[D26] 数组转字符串
来源：http://wbl.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://nlb.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://ezo.shzxlz.cn

JS:   arr.join(", ")
来源：http://lrv.yangfankeji.com

TS:   arr.join(", ")
来源：http://thf.zdbjq.cn

Java: String.join(", ", list)
来源：http://fhx.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://ahl.xuanzx.com

Ruby: arr.join(", ")
来源：http://gqc.wangshuangyany.cn

C#:   string.Join(", ", list)
来源：http://jos.nanxuanxn.top

================================================================================
来源：http://hpn.zhaomingkeji.xyz

E. 字符串处理
来源：http://qse.redwolf501.top

================================================================================
来源：http://xyp.epnwcf.com

[E01] 拼接字符串
来源：http://xiu.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jkn.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ags.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fmf.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jqh.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zmh.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qic.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rai.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ewd.ybcxt.top

[E02] 重复字符串
来源：http://gsc.jlsjyb.cn

Py:   "ab" * 3
来源：http://aoz.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://tlw.sxryk.cn

JS:   "ab".repeat(3)
来源：http://gnv.ydzc1.top

TS:   "ab".repeat(3)
来源：http://tpu.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://fel.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://qda.hnqzz.top

Ruby: "ab" * 3
来源：http://jbp.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pot.guannengcc.top

[E03] 截取子串
来源：http://tcm.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kqh.xuetiantiany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cka.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wvb.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://dcx.wangdashe.top

Java: s.substring(1, 4)
来源：http://ezk.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jmj.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://trj.yonumen.top

C#:   s.Substring(1, 3)
来源：http://kuh.xylfe.cn

[E04] 查找子串位置
来源：http://mbn.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://cyf.yj20258888.top

PHP:  strpos($s, "x");
来源：http://gpv.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vax.cashguo.top

TS:   s.indexOf("x")
来源：http://mdl.jinghuilouyu.cn

Java: s.indexOf("x")
来源：http://erh.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://srg.yuxming.cn

Ruby: s.index("x")
来源：http://fpn.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://lid.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://utv.nwbrower.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qtd.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hpe.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uon.daxiang520.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gac.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fdm.fzhhl.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vxe.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xuc.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tlp.dianchejie.cn

[E06] 替换子串
来源：http://slc.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ijg.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://pxs.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fzn.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://ozq.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ive.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jpd.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wpk.redwolf501.top

C#:   s.Replace("a", "b")
来源：http://rru.epnwcf.com

[E07] 按分隔符拆分
来源：http://tyy.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zpm.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://egs.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rsu.chenjidiqi.icu

TS:   s.split(",")
来源：http://hgb.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://baf.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mac.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://qyl.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gvc.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://iaw.jinqigufen.top

Py:   ",".join(items)
来源：http://utq.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://ppd.xziqi.cn

JS:   items.join(",")
来源：http://ggg.sjlbkw.cn

TS:   items.join(",")
来源：http://yeo.yj202588.top

Java: String.join(",", items)
来源：http://ped.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://ycn.snrcjt.cn

Ruby: items.join(",")
来源：http://hga.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://kvo.cheryme.top

[E09] 去除所有空白字符
来源：http://pyo.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://idq.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://trn.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://slw.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://bgs.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://gnj.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://xrx.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wkt.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://odc.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://eyl.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gnr.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uvh.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://ogy.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://znx.wangdashe.top

Java: String.format("%03d", 7)
来源：http://zpk.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://frj.yueranfly.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dli.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qhe.jlsjyb.cn

[E11] 反转字符串
来源：http://hcq.fanxiaobao.xyz

Py:   s[::-1]
来源：http://rew.nanxuanxn.top

PHP:  strrev($s);
来源：http://kll.cheryme.top

JS:   [...s].reverse().join("")
来源：http://gjt.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://qei.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wkk.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jxt.hywenlv.cn

Ruby: s.reverse
来源：http://hzp.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://riy.nwbrower.top

[E12] 统计某字符出现次数
来源：http://ycr.zhijiandao.cn

Py:   s.count("a")
来源：http://tly.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://ozf.sxryk.cn

JS:   s.split("a").length - 1
来源：http://vom.mhx1999.top

TS:   s.split("a").length - 1
来源：http://liw.shanyushiyangtech.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tqd.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://rjc.cqqwz.cn

Ruby: s.count("a")
来源：http://mwr.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://jki.dashuyun.cn

[E13] 逐字符遍历
来源：http://svk.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://woo.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mky.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nhk.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lcg.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mfk.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://siz.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rwq.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uso.tanke756.top

[E14] URL 编码与 Base64
来源：http://ayc.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jvb.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vem.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aep.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nmd.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cfy.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rqy.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pbv.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fzr.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://jrp.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xob.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hum.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://irg.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mzq.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xiy.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ceu.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ewh.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gwv.gaohongyu789.top

[E16] 数字千分位
来源：http://qlx.gzhubu.top

Py:   f"{1234567:,}"
来源：http://fuj.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://wne.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wyl.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://uuo.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sje.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hfn.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wsn.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://vra.yuanzhike.top

[E17] 首字母大写
来源：http://dca.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gvj.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zdv.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uen.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qsb.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jef.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qfl.jiagoushi.top

Ruby: s.capitalize
来源：http://gln.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bpv.uphjek.com

[E18] 模板占位符替换
来源：http://cup.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ccf.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fmb.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://npt.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vnv.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xzn.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iry.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zug.ydjk.org.cn


<!-- 参考信息 -->