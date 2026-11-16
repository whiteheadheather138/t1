代发 wailian999

[D11] 反转数组
来源：http://gvl.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://ihc.wangdashe.top

PHP:  array_reverse($arr);
来源：http://gez.ybcxt.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uji.yonumen.top

TS:   [...arr].reverse();
来源：http://gfa.fehbvm.com

Java: Collections.reverse(list);
来源：http://any.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://gqo.chenzaomai.com

Ruby: arr.reverse
来源：http://lbz.zdqjudy.top

C#:   list.Reverse();
来源：http://nki.aizwys.cn

[D12] 查找元素下标
来源：http://zve.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://qlh.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jcf.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qvn.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://upm.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zoq.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://kwc.hysaishi.cn

Ruby: arr.index(x)
来源：http://lly.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://mgp.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://tzh.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nli.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://loz.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://cle.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://zaq.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vmm.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qwn.cucudq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wii.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eev.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://kef.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://evf.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ldb.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://wxk.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://pba.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mzk.fanxiaobao.xyz

Go:   // 手写循环
来源：http://wvk.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://ziy.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://ljy.yanxiufei.cn

[D15] 去重
来源：http://rrt.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cnb.shzxlz.cn

PHP:  array_unique($arr);
来源：http://jht.zycfv.cn

JS:   [...new Set(arr)]
来源：http://fli.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://rcc.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://byf.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://xhc.zdbjq.cn

Ruby: arr.uniq
来源：http://gan.yj202588.top

C#:   list.Distinct().ToList()
来源：http://qlv.svipenyu.cn

[D16] 求和与平均值
来源：http://pbc.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ukc.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://spn.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wwp.cdnleiting.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bge.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xhx.sweek.top

Go:   // 手写循环累加
来源：http://neb.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wpb.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://txr.ywan-chungtsiang.top

[D17] 最大值与最小值
来源：http://rrm.tarul.cn

Py:   max(arr);  min(arr)
来源：http://alb.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://sxa.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vmx.yfazqb.com

TS:   Math.max(...arr);
来源：http://lgw.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://xyu.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vuf.hammf.cn

Ruby: arr.max;  arr.min
来源：http://pey.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://zpt.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://jne.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sig.birdmap.top

PHP:  array_merge(...$nested);
来源：http://bkt.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ujl.xuanzx.com

TS:   nested.flat();
来源：http://qqp.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lzd.hesvh.cn

Go:   // 手写双层循环
来源：http://rmk.daria6918.cn

Ruby: nested.flatten
来源：http://izs.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dtz.shanyushiyangtech.top

[D19] 按字段分组
来源：http://aed.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rpt.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sxg.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mku.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rzx.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vld.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://hoy.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pqb.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ial.sjlbkw.cn

[D20] 统计每个元素出现次数
来源：http://xpc.chenjidiqi.icu

Py:   Counter(arr)
来源：http://cts.yj20258.top

PHP:  array_count_values($arr);
来源：http://sfs.jlsjyb.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kve.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hoz.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jgb.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://gmi.shanyushiyangtech.top

Ruby: arr.tally
来源：http://nay.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kfi.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://rxw.mhx1999.top

Py:   x in arr
来源：http://ios.quarkkingdee.top

PHP:  in_array($x, $arr, true);
来源：http://ipy.yuanzhike.top

JS:   arr.includes(x)
来源：http://skk.ybcxt.top

TS:   arr.includes(x)
来源：http://tvg.yj202588.top

Java: list.contains(x)
来源：http://lyi.aibaodan.cn

Go:   slices.Contains(arr, x)
来源：http://pkf.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://ycs.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://tmg.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://irp.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oyj.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rsa.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jsd.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://wff.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://tst.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://eeb.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://oyu.zhixingplan.top

C#:   new List<int>(list);
来源：http://tej.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://mns.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xlj.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vue.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bfj.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dnf.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lcr.hysaishi.cn

Go:   // 手写循环
来源：http://dbv.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://imh.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://frx.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://aig.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ohv.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ocv.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qpb.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ntt.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cxu.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://llo.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eys.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oap.pycfn.com

[D25] Set 集合去重与交并差
来源：http://rly.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uwd.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wck.316326.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://glr.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fuo.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qmo.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://osb.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hpg.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tkj.ydzc1.top

[D26] 数组转字符串
来源：http://nyz.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://phq.pycfn.com

PHP:  implode(", ", $arr);
来源：http://ukv.yueranfly.top

JS:   arr.join(", ")
来源：http://zno.fengsongda.top

TS:   arr.join(", ")
来源：http://alr.yj20258.top

Java: String.join(", ", list)
来源：http://fub.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://gub.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://ekf.cashguo.top

C#:   string.Join(", ", list)
来源：http://rme.zdqjudy.top

================================================================================
来源：http://iaj.yangfankeji.com

E. 字符串处理
来源：http://nvx.jinyuanbaomall.cn

================================================================================
来源：http://zyj.316326.xyz

[E01] 拼接字符串
来源：http://tbm.ydjk.org.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qxz.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mpc.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnq.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dim.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://clr.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mjb.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pnp.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yio.chenjidiqi.icu

[E02] 重复字符串
来源：http://tix.ydzc1.top

Py:   "ab" * 3
来源：http://wbk.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://amf.havefunace.top

JS:   "ab".repeat(3)
来源：http://ecr.hnqzz.top

TS:   "ab".repeat(3)
来源：http://sko.fzhhl.top

Java: "ab".repeat(3)
来源：http://fyz.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://svs.vehdjk.com

Ruby: "ab" * 3
来源：http://udq.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ncu.shuidangran.top

[E03] 截取子串
来源：http://zqa.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ygz.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ixh.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uqv.yfazqb.com

TS:   s.slice(1, 4)
来源：http://myg.yuanzhike.top

Java: s.substring(1, 4)
来源：http://ljz.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yuz.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ubs.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://gzl.chenlongwang.top

[E04] 查找子串位置
来源：http://kxu.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://wma.fengsongda.top

PHP:  strpos($s, "x");
来源：http://aou.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nhx.xylfe.cn

TS:   s.indexOf("x")
来源：http://fht.xinyue.icu

Java: s.indexOf("x")
来源：http://rtc.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://eal.jqgufenzy.top

Ruby: s.index("x")
来源：http://aae.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://rjy.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uzl.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sqi.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iyr.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pqy.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ipz.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nto.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://loj.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bbt.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wwr.iojbl.cn

[E06] 替换子串
来源：http://lty.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qfd.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://udf.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kxa.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://vwu.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://byp.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gti.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pwk.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://yuj.jinghuilouyu.cn

[E07] 按分隔符拆分
来源：http://wxt.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qre.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lzj.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://cad.gotoacloud.top

TS:   s.split(",")
来源：http://msu.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vvx.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hod.yuxming.cn

Ruby: s.split(",");  s.split
来源：http://ejm.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xvp.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://grg.vqdsnc.cn

Py:   ",".join(items)
来源：http://oml.pycfn.com

PHP:  implode(",", $items);
来源：http://ucy.zhoulong.xyz

JS:   items.join(",")
来源：http://zpz.meibo888.top

TS:   items.join(",")
来源：http://ulb.gzhubu.top

Java: String.join(",", items)
来源：http://jcs.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://oxz.xinyue.icu

Ruby: items.join(",")
来源：http://yfc.andypj.xyz

C#:   string.Join(",", items)
来源：http://rsl.yueranfly.top

[E09] 去除所有空白字符
来源：http://aqz.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://imq.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xuh.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://qim.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://dve.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://xgz.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zdd.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ije.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nin.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://mkj.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lpk.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://olc.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://fiw.sufxvd.cn

TS:   "7".padStart(3, "0")
来源：http://aks.wangdashe.top

Java: String.format("%03d", 7)
来源：http://tos.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dym.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://csz.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bvm.chenzaomai.com

[E11] 反转字符串
来源：http://dfv.52xcode.cn

Py:   s[::-1]
来源：http://wey.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://ucl.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://xez.birdmap.top

TS:   [...s].reverse().join("")
来源：http://afs.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ros.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yru.guowangkeji.top

Ruby: s.reverse
来源：http://nbw.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://qtc.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://bzw.meibo888.top

Py:   s.count("a")
来源：http://jaj.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://wwp.zycfv.cn

JS:   s.split("a").length - 1
来源：http://wzd.tian-w.cn

TS:   s.split("a").length - 1
来源：http://bnd.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mfh.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://iev.fzhhl.top

Ruby: s.count("a")
来源：http://pxq.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://ega.vehdjk.com

[E13] 逐字符遍历
来源：http://keo.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://bjh.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pdi.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wrr.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://gjo.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ijh.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ipv.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qgk.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vsu.smart0.xyz

[E14] URL 编码与 Base64
来源：http://opg.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dnc.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vik.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iil.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xbs.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ztl.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://juw.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dal.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xoj.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://cbu.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://mhe.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bsh.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wyr.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://xhd.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rul.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vcb.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://agz.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kei.snrcjt.cn

[E16] 数字千分位
来源：http://rcs.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://ngi.fktsv.cn

PHP:  number_format(1234567);
来源：http://bpz.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ear.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://avo.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dlv.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ovn.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jnu.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://mpe.yuxming.cn

[E17] 首字母大写
来源：http://kic.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://umc.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cdz.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zwd.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dcu.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zrf.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://whx.gotoacloud.top

Ruby: s.capitalize
来源：http://eif.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tts.bjfxy.top


<!-- 参考信息 -->