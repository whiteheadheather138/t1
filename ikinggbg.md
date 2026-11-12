代发 wailian999

C#:   list.Reverse();
来源：http://vfm.jinqigfzy.top

[D12] 查找元素下标
来源：http://vgn.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://wcv.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uxu.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pzr.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mmi.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yfj.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://sjl.yj20258888.top

Ruby: arr.index(x)
来源：http://epv.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://utv.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://iqb.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fyg.sysykeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ell.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://piz.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://mng.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://egp.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ebi.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://urx.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://csx.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://gcp.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://obr.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://chw.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://pns.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://lua.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oow.nwbrower.top

Go:   // 手写循环
来源：http://rli.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://zft.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ymr.sweek.top

[D15] 去重
来源：http://yyz.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kfa.52xcode.cn

PHP:  array_unique($arr);
来源：http://tmo.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://keb.meibo888.top

TS:   [...new Set(arr)]
来源：http://xao.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xnt.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ccz.hywenlv.cn

Ruby: arr.uniq
来源：http://qge.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://vgk.nanxuanxn.top

[D16] 求和与平均值
来源：http://ygf.xingfuxueyuan.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rap.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sfg.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xlm.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xjm.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lmk.zycfv.cn

Go:   // 手写循环累加
来源：http://jgw.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ohc.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://wnh.jlsjyb.cn

[D17] 最大值与最小值
来源：http://ing.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://azn.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://swl.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://itj.shzxlz.cn

TS:   Math.max(...arr);
来源：http://ogd.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zlx.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bqx.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://ufa.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://fyh.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://byi.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zgj.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://flb.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nbt.daxiang520.top

TS:   nested.flat();
来源：http://wau.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ckw.ehwqpu.com

Go:   // 手写双层循环
来源：http://kng.guowangkeji.top

Ruby: nested.flatten
来源：http://qtv.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yjp.zhijiandao.cn

[D19] 按字段分组
来源：http://bve.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mhm.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wqd.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kbb.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cam.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vqc.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://irc.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://umq.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wsf.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://mll.cqqwz.cn

Py:   Counter(arr)
来源：http://bhs.tarul.cn

PHP:  array_count_values($arr);
来源：http://fwe.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sef.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gvb.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://myu.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://sts.shzxlz.cn

Ruby: arr.tally
来源：http://dpi.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wjo.yongpay.top

[D21] 判断是否包含某元素
来源：http://skl.chenjidiqi.icu

Py:   x in arr
来源：http://rod.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://qxe.hnqzz.top

JS:   arr.includes(x)
来源：http://uic.kuanghao11.cn

TS:   arr.includes(x)
来源：http://zdv.mhx1999.top

Java: list.contains(x)
来源：http://pha.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://lcg.yueranfly.top

Ruby: arr.include?(x)
来源：http://pfz.yanxiufei.cn

C#:   list.Contains(x)
来源：http://efa.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://uwp.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://brj.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zpi.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tcs.cashguo.top

TS:   [...arr];
来源：http://ryy.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://nsz.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cdo.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://bua.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://dot.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://sxe.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pqk.cqqwz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fhv.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yup.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kgh.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://etu.jinqigfzy.top

Go:   // 手写循环
来源：http://oiq.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://shs.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dcz.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://mpm.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kkh.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vzx.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oxc.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bzf.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vul.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://twk.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zcb.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dyi.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://lkw.jlsjyb.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dmi.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fxv.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wbs.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zex.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bok.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hkg.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nzm.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xfb.9152youxi.cn

[D26] 数组转字符串
来源：http://zcd.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://wcz.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://orn.zhoulong.xyz

JS:   arr.join(", ")
来源：http://jie.xinyue.icu

TS:   arr.join(", ")
来源：http://eut.cucudq.cn

Java: String.join(", ", list)
来源：http://kzt.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://hqf.hysaishi.cn

Ruby: arr.join(", ")
来源：http://lyv.yuxming.cn

C#:   string.Join(", ", list)
来源：http://dfy.fengsongda.top

================================================================================
来源：http://anw.yueranfly.top

E. 字符串处理
来源：http://yfo.havefunace.top

================================================================================
来源：http://yez.hnxiangtu.top

[E01] 拼接字符串
来源：http://pyt.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jyc.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gpe.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xxz.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fhn.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kmk.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://syx.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rei.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bun.chenjidiqi.icu

[E02] 重复字符串
来源：http://kho.yvedp.cn

Py:   "ab" * 3
来源：http://fmt.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://cfi.sweek.top

JS:   "ab".repeat(3)
来源：http://zul.tanke756.top

TS:   "ab".repeat(3)
来源：http://zdb.mhx1999.top

Java: "ab".repeat(3)
来源：http://uqu.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://tdp.andypj.xyz

Ruby: "ab" * 3
来源：http://qhi.hfpthk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lfx.xziqi.cn

[E03] 截取子串
来源：http://bwu.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yqo.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sbv.nanxuanxn.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://prp.shuidangran.top

TS:   s.slice(1, 4)
来源：http://nmw.52xcode.cn

Java: s.substring(1, 4)
来源：http://qah.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://smr.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://qri.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://aio.yonumen.top

[E04] 查找子串位置
来源：http://mfc.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://tpx.yj20258.top

PHP:  strpos($s, "x");
来源：http://tpd.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hvi.gotoacloud.top

TS:   s.indexOf("x")
来源：http://qjx.andypj.xyz

Java: s.indexOf("x")
来源：http://uxp.meibo888.top

Go:   strings.Index(s, "x")
来源：http://pyr.xylfe.cn

Ruby: s.index("x")
来源：http://qrk.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://ktx.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://shy.hfpthk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fdd.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bdq.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cyv.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wfd.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://buv.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ueg.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cck.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bjo.tanke756.top

[E06] 替换子串
来源：http://ldy.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://noo.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://kor.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mlu.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://hrv.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vnr.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rhv.meibo888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bij.hammf.cn

C#:   s.Replace("a", "b")
来源：http://uln.svipenyu.cn

[E07] 按分隔符拆分
来源：http://hqs.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rdu.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kqz.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vzg.tian-w.cn

TS:   s.split(",")
来源：http://ema.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dwh.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gic.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://rnk.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gle.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://gru.sysykeji.top

Py:   ",".join(items)
来源：http://jrz.guowangkeji.top

PHP:  implode(",", $items);
来源：http://jbz.yj202588.top

JS:   items.join(",")
来源：http://ouk.andypj.xyz

TS:   items.join(",")
来源：http://upa.tanke756.top

Java: String.join(",", items)
来源：http://uyg.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://tnm.yueranfly.top

Ruby: items.join(",")
来源：http://dha.pycfn.com

C#:   string.Join(",", items)
来源：http://hpu.epnwcf.com

[E09] 去除所有空白字符
来源：http://irv.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pjr.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fvx.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://kex.ydjk.org.cn

TS:   s.replace(/\s+/g, "")
来源：http://zmq.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://rxz.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rvy.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://uit.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lkf.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://rir.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ajz.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bgs.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://fws.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://czc.yonumen.top

Java: String.format("%03d", 7)
来源：http://uim.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fzc.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tro.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ezt.haohaochexian.top

[E11] 反转字符串
来源：http://yoy.daria6918.cn

Py:   s[::-1]
来源：http://xhl.guowangkeji.top

PHP:  strrev($s);
来源：http://qut.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://gfv.sysykeji.top

TS:   [...s].reverse().join("")
来源：http://bhe.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ebk.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://qbj.havefunace.top

Ruby: s.reverse
来源：http://yhi.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://uxb.shuidangran.top

[E12] 统计某字符出现次数
来源：http://bgx.yj20258888.top

Py:   s.count("a")
来源：http://rrp.uphjek.com

PHP:  substr_count($s, "a");
来源：http://zsb.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://arz.zycfv.cn

TS:   s.split("a").length - 1
来源：http://qij.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qct.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://xrg.ivvv.top

Ruby: s.count("a")
来源：http://cam.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://muv.haohaochexian.top

[E13] 逐字符遍历
来源：http://onh.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://qlf.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wsy.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jue.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nzr.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xgj.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eac.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yyn.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hpj.gzhubu.top

[E14] URL 编码与 Base64
来源：http://zdq.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gkk.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://opr.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xlu.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mnv.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eau.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gmc.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eac.cqqwz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tam.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://kuc.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://nfz.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://svm.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ibj.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qwk.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://igd.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oeq.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lyh.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mct.tian-w.cn

[E16] 数字千分位
来源：http://hcl.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://lom.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://szp.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tpa.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://syn.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nuq.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pij.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jwa.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://cyy.zhengqikj.top

[E17] 首字母大写
来源：http://xjq.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kyv.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eoy.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://udt.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zej.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fki.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lbs.cqqwz.cn

Ruby: s.capitalize
来源：http://osf.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yic.ehwqpu.com

[E18] 模板占位符替换
来源：http://acl.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ced.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qrh.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fxb.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ptl.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fqj.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mbf.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wwx.tian-w.cn


<!-- 参考信息 -->