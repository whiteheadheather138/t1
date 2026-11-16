代发 wailian999

Ruby: arr.index(x)
来源：http://voc.yj20258.top

C#:   list.IndexOf(x);
来源：http://wdw.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://wpb.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hll.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ngg.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://mxo.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://nti.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ivp.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qzd.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://yyz.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fdi.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://ozt.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tlo.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://klm.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://xtp.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://gru.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ile.fktsv.cn

Go:   // 手写循环
来源：http://azt.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://xjd.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ldl.aizwys.cn

[D15] 去重
来源：http://ijl.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lpa.xuanzx.com

PHP:  array_unique($arr);
来源：http://gkq.zycfv.cn

JS:   [...new Set(arr)]
来源：http://pvf.uphjek.com

TS:   [...new Set(arr)]
来源：http://akp.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://skr.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://uaf.xuetiantiany.cn

Ruby: arr.uniq
来源：http://epc.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://vyi.shangyingyoupin.top

[D16] 求和与平均值
来源：http://rtv.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qwk.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://afq.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lii.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wba.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qsg.jianghu66.top

Go:   // 手写循环累加
来源：http://crn.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tqf.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://eax.zdbjq.cn

[D17] 最大值与最小值
来源：http://gsp.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://idm.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://qmc.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gfb.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://yrl.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jes.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ocm.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://hpw.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://zrb.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://jsr.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hcn.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://crv.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tuq.cashguo.top

TS:   nested.flat();
来源：http://qdg.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fuj.zdqjudy.top

Go:   // 手写双层循环
来源：http://pku.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://azx.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://aji.yfazqb.com

[D19] 按字段分组
来源：http://trs.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ekn.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://axv.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kxc.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zhw.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lyy.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://svi.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tyf.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xic.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://nkd.aizwys.cn

Py:   Counter(arr)
来源：http://zkh.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://oxe.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npy.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ykp.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jkm.fzhhl.top

Go:   // 手写 map[T]int
来源：http://ape.shanyushiyangtech.top

Ruby: arr.tally
来源：http://eio.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tpk.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://clw.hammf.cn

Py:   x in arr
来源：http://dtm.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://jss.jianghu66.top

JS:   arr.includes(x)
来源：http://pja.pycfn.com

TS:   arr.includes(x)
来源：http://ljr.jiagoushi.top

Java: list.contains(x)
来源：http://czl.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://dar.aibaodan.cn

Ruby: arr.include?(x)
来源：http://mpj.aibaodan.cn

C#:   list.Contains(x)
来源：http://xsm.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://goz.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://twf.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rwn.snrcjt.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lvb.shanyushiyangtech.top

TS:   [...arr];
来源：http://jsg.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://uxy.ywan-chungtsiang.top

Go:   copied := append([]int(nil), arr...)
来源：http://scy.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://rjj.wangshuangyany.cn

C#:   new List<int>(list);
来源：http://wpx.dianchejie.cn

[D23] reduce 累积计算
来源：http://vco.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wwm.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hov.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fkc.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ina.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://ihg.yvedp.cn

Go:   // 手写循环
来源：http://del.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jjj.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hxk.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://guh.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nxo.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lzb.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ebm.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iny.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jor.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ffi.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://shp.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hss.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://cbn.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vxm.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wtt.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rey.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sya.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fgl.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bpl.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eth.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xka.nanxuanxn.top

[D26] 数组转字符串
来源：http://tfu.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://dlf.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://vpm.gzhubu.top

JS:   arr.join(", ")
来源：http://qnf.hesvh.cn

TS:   arr.join(", ")
来源：http://blf.jinqigfzy.top

Java: String.join(", ", list)
来源：http://ncd.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://tcd.zycfv.cn

Ruby: arr.join(", ")
来源：http://uln.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://qbe.snrcjt.cn

================================================================================
来源：http://ubr.mhx1999.top

E. 字符串处理
来源：http://uee.fanxiaobao.xyz

================================================================================
来源：http://sub.ivvv.top

[E01] 拼接字符串
来源：http://scf.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zib.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rlr.yangfankeji.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://auh.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vaa.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uad.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ynu.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jzj.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fgy.sjlbkw.cn

[E02] 重复字符串
来源：http://akr.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://ytb.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://gpt.hcnkem.com

JS:   "ab".repeat(3)
来源：http://sga.hammf.cn

TS:   "ab".repeat(3)
来源：http://zxh.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://xdq.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://srj.birdmap.top

Ruby: "ab" * 3
来源：http://nqn.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lnr.pengpengdd.cyou

[E03] 截取子串
来源：http://btl.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oun.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ong.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jrv.yvedp.cn

TS:   s.slice(1, 4)
来源：http://gfz.hysaishi.cn

Java: s.substring(1, 4)
来源：http://qyg.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://usn.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://kce.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://hyk.zdqjudy.top

[E04] 查找子串位置
来源：http://njx.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://hyj.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://wwi.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bys.mhx1999.top

TS:   s.indexOf("x")
来源：http://kna.bbcook.cn

Java: s.indexOf("x")
来源：http://ptz.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://hzz.ybcxt.top

Ruby: s.index("x")
来源：http://dmc.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://van.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://bvl.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vvg.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fpv.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ikk.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fec.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://stn.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://czp.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nvr.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ldl.hfpthk.cn

[E06] 替换子串
来源：http://ugf.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pki.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://brm.wangshuangyany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iaj.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://ubt.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gse.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pvo.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ptr.316326.xyz

C#:   s.Replace("a", "b")
来源：http://epy.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://ktp.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zvl.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mam.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ecf.daxiang520.top

TS:   s.split(",")
来源：http://ddc.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jno.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mok.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://zwo.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vtr.52xcode.cn

[E08] 数组按分隔符合并
来源：http://pet.hnqzz.top

Py:   ",".join(items)
来源：http://eob.chenzaomai.com

PHP:  implode(",", $items);
来源：http://utv.jianghu66.top

JS:   items.join(",")
来源：http://lqo.cheryme.top

TS:   items.join(",")
来源：http://tgp.jqgfzy.top

Java: String.join(",", items)
来源：http://bld.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://vyb.ivvv.top

Ruby: items.join(",")
来源：http://rxh.jianghu66.top

C#:   string.Join(",", items)
来源：http://dgi.yuanzhike.top

[E09] 去除所有空白字符
来源：http://gca.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tpd.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rak.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://fkl.tianlin.xyz

TS:   s.replace(/\s+/g, "")
来源：http://qon.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://ogu.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vhp.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://lcj.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gqx.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://cwl.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ooc.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bup.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://mns.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://pwq.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://ewy.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://roq.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://evd.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://maf.ivvv.top

[E11] 反转字符串
来源：http://flk.wangshuangyany.cn

Py:   s[::-1]
来源：http://svk.hysaishi.cn

PHP:  strrev($s);
来源：http://csj.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://qoo.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://swy.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ign.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://svu.pengpengdd.cyou

Ruby: s.reverse
来源：http://xnq.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://ggg.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://mij.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://uwi.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://kuj.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://zpo.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://bfd.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gaq.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://qhy.xinyue.icu

Ruby: s.count("a")
来源：http://ntm.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://mey.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://pzs.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://dpr.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vyg.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mtu.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://fsy.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://czn.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://agg.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://lqw.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gdl.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://jpa.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mse.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xzr.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gcf.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oeg.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lpt.ywan-chungtsiang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rvz.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ulj.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yse.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://vra.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ocm.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://goz.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fat.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xgy.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qda.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mqq.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lvq.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uim.fanxiaobao.xyz

[E16] 数字千分位
来源：http://xkk.gzhubu.top

Py:   f"{1234567:,}"
来源：http://lut.iojbl.cn

PHP:  number_format(1234567);
来源：http://epf.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qfy.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://anm.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nnr.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ses.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vxf.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://jhh.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://csq.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ogc.gzhubu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cgr.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lhz.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://htr.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pdd.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tvk.feifeiyinyue.top

Ruby: s.capitalize
来源：http://ptv.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rzm.vehdjk.com

[E18] 模板占位符替换
来源：http://mcy.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hox.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ntt.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vxu.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xss.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fjm.shangyingyoupin.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zae.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wbf.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uwy.daxiang520.top

[E19] 多行文本按行拆分
来源：http://ogb.gogol.net.cn

Py:   s.splitlines()
来源：http://rpz.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iiz.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://gbh.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://fnl.redwolf501.top

Java: s.lines().toList()
来源：http://mpv.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://qbg.xziqi.cn


<!-- 参考信息 -->