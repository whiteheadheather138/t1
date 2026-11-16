代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cmu.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kmx.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ojd.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://bum.tarul.cn

Ruby: arr.index(x)
来源：http://fvi.vehdjk.com

C#:   list.IndexOf(x);
来源：http://zki.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://hnd.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uto.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qdv.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://cea.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://beg.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://joj.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ljh.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tsi.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://zqr.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://ywf.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://crw.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mlw.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://ruo.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://phx.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ter.vehdjk.com

Go:   // 手写循环
来源：http://iau.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://sfi.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://buo.fehbvm.com

[D15] 去重
来源：http://gsr.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lhq.gzhubu.top

PHP:  array_unique($arr);
来源：http://vsg.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://qnt.tarul.cn

TS:   [...new Set(arr)]
来源：http://vpx.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mel.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fib.fengsongda.top

Ruby: arr.uniq
来源：http://css.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://ird.yongpay.top

[D16] 求和与平均值
来源：http://ted.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hsl.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cqx.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jcg.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://trr.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gpf.fehbvm.com

Go:   // 手写循环累加
来源：http://mlk.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qzq.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://sim.jinqigufen.top

[D17] 最大值与最小值
来源：http://zig.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://sdd.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://rhf.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gly.jqgfzy.top

TS:   Math.max(...arr);
来源：http://uds.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://srk.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fbf.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://pbs.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://cvw.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://lti.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://arv.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://mjr.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rke.sufxvd.cn

TS:   nested.flat();
来源：http://bnh.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jid.nanxuanxn.top

Go:   // 手写双层循环
来源：http://heu.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://dop.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ghh.quarkkingdee.top

[D19] 按字段分组
来源：http://rux.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wqk.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ewh.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gku.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gca.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kdw.snrcjt.cn

Go:   // 手写 map[string][]T
来源：http://yxm.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hnc.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dxk.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://iky.xylfe.cn

Py:   Counter(arr)
来源：http://mop.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://hfl.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cwj.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aze.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hpi.jianghu66.top

Go:   // 手写 map[T]int
来源：http://ybv.guowangkeji.top

Ruby: arr.tally
来源：http://bzg.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://teh.yonumen.top

[D21] 判断是否包含某元素
来源：http://cqg.feifeiyinyue.top

Py:   x in arr
来源：http://pgd.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://tis.jinqigufen.top

JS:   arr.includes(x)
来源：http://pvl.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://cia.fehbvm.com

Java: list.contains(x)
来源：http://kuc.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://mhs.jyoumei.cn

Ruby: arr.include?(x)
来源：http://qoe.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://ovq.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://bde.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ier.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pqm.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yqm.aizwys.cn

TS:   [...arr];
来源：http://okz.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://gda.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qws.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://ydx.havefunace.top

C#:   new List<int>(list);
来源：http://hxj.smart0.xyz

[D23] reduce 累积计算
来源：http://uqw.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cmf.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eye.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://irw.meibo888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mfb.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://otw.vqdsnc.cn

Go:   // 手写循环
来源：http://mjq.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cpi.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nml.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://qxh.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pla.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wut.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://btt.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ple.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hzq.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://onm.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ecr.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bhn.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://whg.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://myn.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rfb.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zie.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zyb.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wrl.ivvv.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ann.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qhz.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mtf.svipenyu.cn

[D26] 数组转字符串
来源：http://blp.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://yil.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://agl.nanxinkj.top

JS:   arr.join(", ")
来源：http://ina.shangyingyoupin.top

TS:   arr.join(", ")
来源：http://zkj.haohaochexian.top

Java: String.join(", ", list)
来源：http://pey.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://eio.dianchejie.cn

Ruby: arr.join(", ")
来源：http://bpm.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://psw.snrcjt.cn

================================================================================
来源：http://htx.jqgfzy.top

E. 字符串处理
来源：http://wfz.meibo888.top

================================================================================
来源：http://lvy.redwolf501.top

[E01] 拼接字符串
来源：http://fah.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sam.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://elx.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fsx.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bta.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://grs.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gfr.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zng.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xlw.tian-w.cn

[E02] 重复字符串
来源：http://rjy.sweek.top

Py:   "ab" * 3
来源：http://mlv.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://idw.havefunace.top

JS:   "ab".repeat(3)
来源：http://tkf.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://grz.yfazqb.com

Java: "ab".repeat(3)
来源：http://bmf.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://uaa.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://nfg.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qxv.sufxvd.cn

[E03] 截取子串
来源：http://vvo.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yyd.dashuyun.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kmz.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ldn.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://lsa.hnqzz.top

Java: s.substring(1, 4)
来源：http://orx.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tdo.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ocf.shzxlz.cn

C#:   s.Substring(1, 3)
来源：http://hzc.haohaochexian.top

[E04] 查找子串位置
来源：http://lfq.yuxming.cn

Py:   s.find("x");  s.index("x")
来源：http://fib.xylfe.cn

PHP:  strpos($s, "x");
来源：http://bfk.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://khv.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://pgx.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://zwk.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://axr.svipenyu.cn

Ruby: s.index("x")
来源：http://ktf.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://klr.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://exh.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jlo.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uks.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zxz.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://skl.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fdg.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://psn.daxiang520.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zhw.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ayi.hcnkem.com

[E06] 替换子串
来源：http://rnb.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jgq.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://erj.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mjd.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://kzm.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ysy.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pfr.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zxh.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://asw.fehbvm.com

[E07] 按分隔符拆分
来源：http://rxr.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ddt.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xsy.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qno.guannengcc.top

TS:   s.split(",")
来源：http://svi.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fio.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xfa.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://krg.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kna.gzhubu.top

[E08] 数组按分隔符合并
来源：http://qkl.tianlin.xyz

Py:   ",".join(items)
来源：http://ntq.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://wop.yueranfly.top

JS:   items.join(",")
来源：http://utm.jqgufenzy.top

TS:   items.join(",")
来源：http://vvd.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://zaf.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://fnd.vqdsnc.cn

Ruby: items.join(",")
来源：http://kdv.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://chj.snrcjt.cn

[E09] 去除所有空白字符
来源：http://fuj.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gsc.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ttr.fengsongda.top

JS:   s.replace(/\s+/g, "")
来源：http://zji.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://rpc.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://qbh.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nau.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://arx.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://glu.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://fsw.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fax.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hhv.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://shs.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://nuf.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://hmj.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aho.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ivb.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hzs.aizwys.cn

[E11] 反转字符串
来源：http://lsz.sxryk.cn

Py:   s[::-1]
来源：http://vbe.havefunace.top

PHP:  strrev($s);
来源：http://hci.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://hyn.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://hks.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mcc.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kww.nanxinkj.top

Ruby: s.reverse
来源：http://kwx.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://yhh.cashguo.top

[E12] 统计某字符出现次数
来源：http://xbb.shangyingyoupin.top

Py:   s.count("a")
来源：http://nbo.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://kmg.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://dvw.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://gqp.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ngg.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://vcs.cqqwz.cn

Ruby: s.count("a")
来源：http://ldd.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://glq.ybcxt.top

[E13] 逐字符遍历
来源：http://lhr.meibo888.top

Py:   for ch in s: print(ch)
来源：http://ile.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://irg.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jvl.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rcn.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lzm.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nsn.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mir.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://glq.xylfe.cn

[E14] URL 编码与 Base64
来源：http://jvh.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sdm.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xom.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dxq.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bge.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hnn.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ubt.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://coe.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rha.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://xtf.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mln.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blf.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rbc.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iyi.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mki.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://her.0kj1m.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kad.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gvf.gaohongyu789.top

[E16] 数字千分位
来源：http://xmm.meibo888.top

Py:   f"{1234567:,}"
来源：http://aqb.chenzaomai.com

PHP:  number_format(1234567);
来源：http://uzk.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://nkl.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wiy.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jva.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vqr.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fnv.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://usv.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://vgc.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ppb.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gzo.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oci.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aor.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sod.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zcb.yangfankeji.com

Ruby: s.capitalize
来源：http://sfy.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iiz.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://svu.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nfc.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dgj.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://flh.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wbs.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mme.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vgz.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vro.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yab.yfazqb.com

[E19] 多行文本按行拆分
来源：http://axo.316326.xyz

Py:   s.splitlines()
来源：http://ebf.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hxk.zhoulong.xyz


<!-- 参考信息 -->