代发 wailian999

TS:   [...arr].reverse();
来源：http://nff.yueranfly.top

Java: Collections.reverse(list);
来源：http://peb.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://tao.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://hqw.fengsongda.top

C#:   list.Reverse();
来源：http://sxm.iojbl.cn

[D12] 查找元素下标
来源：http://ofg.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://tmz.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pcr.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ooj.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qpy.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://agu.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://rfx.ppjwa.cn

Ruby: arr.index(x)
来源：http://nrh.yfazqb.com

C#:   list.IndexOf(x);
来源：http://ntw.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://dan.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lec.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rqa.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://rzp.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://cjm.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nub.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ojb.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://jqm.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://biq.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://rza.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cbi.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tho.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://hvv.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://gmw.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lqw.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://yhv.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gio.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://paw.gotoacloud.top

[D15] 去重
来源：http://ybz.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://agg.meibo888.top

PHP:  array_unique($arr);
来源：http://ybq.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://gzq.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://tef.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ccc.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://qqp.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://exq.uphjek.com

C#:   list.Distinct().ToList()
来源：http://zfj.shzxlz.cn

[D16] 求和与平均值
来源：http://sxs.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vla.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qzf.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sun.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tdq.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ewi.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://wub.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gko.hnxiangtu.top

C#:   list.Sum();  list.Average()
来源：http://anr.hammf.cn

[D17] 最大值与最小值
来源：http://aqh.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://kyy.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://zus.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cvq.snrcjt.cn

TS:   Math.max(...arr);
来源：http://sew.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://clb.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zig.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://bov.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://swo.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://yxg.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pjo.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://yua.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://orn.fzhhl.top

TS:   nested.flat();
来源：http://vav.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lwi.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://hos.yongpay.top

Ruby: nested.flatten
来源：http://vpo.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vrn.hnxiangtu.top

[D19] 按字段分组
来源：http://xey.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ash.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iwa.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hav.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eqc.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nhb.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://ozx.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tim.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fxu.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://otw.svipenyu.cn

Py:   Counter(arr)
来源：http://bhl.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://qab.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://huu.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yyh.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bxu.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://lee.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://vfm.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wum.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://rsx.zhiwuduotai.top

Py:   x in arr
来源：http://jvn.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://nyt.cqqwz.cn

JS:   arr.includes(x)
来源：http://sla.snrcjt.cn

TS:   arr.includes(x)
来源：http://gwx.smart0.xyz

Java: list.contains(x)
来源：http://vyd.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://cfz.meibo888.top

Ruby: arr.include?(x)
来源：http://fgz.zhoulong.xyz

C#:   list.Contains(x)
来源：http://vui.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://ypn.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wby.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pql.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cce.nanxinkj.top

TS:   [...arr];
来源：http://nit.iojbl.cn

Java: new ArrayList<>(list);
来源：http://lww.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://qtf.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://cyc.zhongyouzk.top

C#:   new List<int>(list);
来源：http://foi.mhx1999.top

[D23] reduce 累积计算
来源：http://oav.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zob.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://znu.fehbvm.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vwn.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qai.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://dfs.nwbrower.top

Go:   // 手写循环
来源：http://uls.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tdd.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cxk.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://vkn.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cxf.nwbrower.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xwb.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://okw.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hbu.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jpg.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pem.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://shs.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hif.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://nkt.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kjw.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lcb.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kgi.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kvn.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tcc.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bib.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kvz.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ael.zhiwuduotai.top

[D26] 数组转字符串
来源：http://alw.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://mal.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://tax.tian-w.cn

JS:   arr.join(", ")
来源：http://jxm.xylfe.cn

TS:   arr.join(", ")
来源：http://cfu.c1oappe.top

Java: String.join(", ", list)
来源：http://fml.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://grj.mhx1999.top

Ruby: arr.join(", ")
来源：http://hvi.smart0.xyz

C#:   string.Join(", ", list)
来源：http://aaw.birdmap.top

================================================================================
来源：http://uyb.316326.xyz

E. 字符串处理
来源：http://ssd.iojbl.cn

================================================================================
来源：http://uzc.yj20258888.top

[E01] 拼接字符串
来源：http://tdx.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://njc.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uuq.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://udh.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mly.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://opt.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kxk.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lkn.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jet.nanxuanxn.top

[E02] 重复字符串
来源：http://mhz.yj202588.top

Py:   "ab" * 3
来源：http://dyg.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://pfk.fengsongda.top

JS:   "ab".repeat(3)
来源：http://dbg.andypj.xyz

TS:   "ab".repeat(3)
来源：http://dwe.yonumen.top

Java: "ab".repeat(3)
来源：http://iff.wangdashe.top

Go:   strings.Repeat("ab", 3)
来源：http://dkg.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://lib.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rzj.iojbl.cn

[E03] 截取子串
来源：http://lve.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://par.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hbf.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blx.fzhhl.top

TS:   s.slice(1, 4)
来源：http://dne.gotoacloud.top

Java: s.substring(1, 4)
来源：http://toc.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rip.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://css.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://jun.ydzc1.top

[E04] 查找子串位置
来源：http://hgr.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://dqn.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://utm.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wkq.cashguo.top

TS:   s.indexOf("x")
来源：http://pax.xuanzx.com

Java: s.indexOf("x")
来源：http://hty.cashguo.top

Go:   strings.Index(s, "x")
来源：http://rre.hfpthk.cn

Ruby: s.index("x")
来源：http://tjk.fktsv.cn

C#:   s.IndexOf("x")
来源：http://tev.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dxg.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://shg.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://myt.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nwe.hywenlv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sgt.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mnw.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pfb.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://szm.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eni.sxryk.cn

[E06] 替换子串
来源：http://hqy.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wcx.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://yva.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xhq.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://nig.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dlw.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pod.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ntx.birdmap.top

C#:   s.Replace("a", "b")
来源：http://sfe.52xcode.cn

[E07] 按分隔符拆分
来源：http://xxy.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jsw.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aen.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tjg.kuanghao11.cn

TS:   s.split(",")
来源：http://jve.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://uvj.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sgm.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://qcn.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sfh.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://tuw.mhx1999.top

Py:   ",".join(items)
来源：http://bnc.havefunace.top

PHP:  implode(",", $items);
来源：http://kqp.zycfv.cn

JS:   items.join(",")
来源：http://iko.sweek.top

TS:   items.join(",")
来源：http://wnq.zdbjq.cn

Java: String.join(",", items)
来源：http://eez.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://mgp.chenjidiqi.icu

Ruby: items.join(",")
来源：http://nlj.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://fgt.hnqzz.top

[E09] 去除所有空白字符
来源：http://lim.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aby.cashguo.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://clw.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://vfj.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://ctp.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://hib.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://auk.kuanghao11.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hbg.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fnl.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://agv.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://naf.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ngv.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://jcd.sweek.top

TS:   "7".padStart(3, "0")
来源：http://zfx.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://gtb.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://vaj.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jiy.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fas.yongpay.top

[E11] 反转字符串
来源：http://wex.zdqjudy.top

Py:   s[::-1]
来源：http://lft.tian-w.cn

PHP:  strrev($s);
来源：http://moz.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://lsl.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://bfr.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ocd.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://njg.hysaishi.cn

Ruby: s.reverse
来源：http://rvo.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://bco.aizwys.cn

[E12] 统计某字符出现次数
来源：http://xtx.ybcxt.top

Py:   s.count("a")
来源：http://zif.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://vup.sxryk.cn

JS:   s.split("a").length - 1
来源：http://fna.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://tjk.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xvc.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://szo.9152youxi.cn

Ruby: s.count("a")
来源：http://ayv.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://apq.52xcode.cn

[E13] 逐字符遍历
来源：http://cqg.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://tvq.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tbl.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://dlx.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qrb.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iaw.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tng.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://imq.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nvo.bjfxy.top

[E14] URL 编码与 Base64
来源：http://ipq.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qnr.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fiu.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ogj.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lsg.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://die.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oja.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bsl.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aam.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://koh.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nex.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yhq.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zhd.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lua.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ifc.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sxo.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ilx.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wda.hywenlv.cn

[E16] 数字千分位
来源：http://pic.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://cay.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://tdp.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pwv.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vab.haohaochexian.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ctc.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tmt.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://whp.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://lxh.sweek.top

[E17] 首字母大写
来源：http://xfz.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wpg.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xps.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uln.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jgc.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bqf.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gss.ppjwa.cn

Ruby: s.capitalize
来源：http://wdf.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ehz.dashuyun.cn

[E18] 模板占位符替换
来源：http://vxr.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://spk.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qvy.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xjj.vqdsnc.cn


<!-- 参考信息 -->