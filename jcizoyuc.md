代发 wailian999

C#:   list.Reverse();
来源：http://kmy.yj20258.top

[D12] 查找元素下标
来源：http://wtq.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://oul.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xyo.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kcg.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://epc.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gvg.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://slj.meibo888.top

Ruby: arr.index(x)
来源：http://nem.daria6918.cn

C#:   list.IndexOf(x);
来源：http://wle.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://ytv.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://loi.bjfxy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qlp.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://inv.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://imx.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zzy.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wlj.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://ypz.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zaf.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://fdy.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iif.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jap.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://efh.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://pja.fktsv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wjj.feifeiyinyue.top

Go:   // 手写循环
来源：http://wcz.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://hgs.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://iid.ybcxt.top

[D15] 去重
来源：http://ile.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rom.iojbl.cn

PHP:  array_unique($arr);
来源：http://efr.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://oct.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://kft.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yzd.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lhr.tanke756.top

Ruby: arr.uniq
来源：http://jnv.aizwys.cn

C#:   list.Distinct().ToList()
来源：http://ipr.fktsv.cn

[D16] 求和与平均值
来源：http://fhs.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zbp.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gxt.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://btw.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tyb.sweek.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jpu.chenlongwang.top

Go:   // 手写循环累加
来源：http://uop.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mul.hnxiangtu.top

C#:   list.Sum();  list.Average()
来源：http://tqe.kuanghao11.cn

[D17] 最大值与最小值
来源：http://err.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://zig.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://qkh.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wla.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://fyf.ywan-chungtsiang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nct.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yxk.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://syi.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://hzv.uphjek.com

[D18] 扁平化嵌套数组
来源：http://ryz.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bio.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://yaf.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ibs.52xcode.cn

TS:   nested.flat();
来源：http://oab.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wjw.xziqi.cn

Go:   // 手写双层循环
来源：http://vqd.gaohongyu789.top

Ruby: nested.flatten
来源：http://psx.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jwp.yj20258.top

[D19] 按字段分组
来源：http://gqx.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://riq.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://juo.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dmr.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iei.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://scu.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://rjb.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://mee.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mlo.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://oun.chenlongwang.top

Py:   Counter(arr)
来源：http://tos.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://npe.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rlt.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dyv.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dpw.fzhhl.top

Go:   // 手写 map[T]int
来源：http://zys.birdmap.top

Ruby: arr.tally
来源：http://low.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eah.xylfe.cn

[D21] 判断是否包含某元素
来源：http://scd.jinqigufen.top

Py:   x in arr
来源：http://jnh.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://ssx.birdmap.top

JS:   arr.includes(x)
来源：http://xhs.hammf.cn

TS:   arr.includes(x)
来源：http://kjr.ybcxt.top

Java: list.contains(x)
来源：http://uwx.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://yig.ivvv.top

Ruby: arr.include?(x)
来源：http://wfl.nanxuanxn.top

C#:   list.Contains(x)
来源：http://ftq.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://ipc.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://era.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vmt.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zzl.fanxiaobao.xyz

TS:   [...arr];
来源：http://sji.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://hzc.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://ytl.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://uwa.havefunace.top

C#:   new List<int>(list);
来源：http://rxz.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://mlc.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://okz.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wao.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ocw.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xww.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://boq.yj20258888.top

Go:   // 手写循环
来源：http://esy.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mlv.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sty.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://pxf.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://knv.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qam.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jgh.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cnk.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jia.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ltz.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dxu.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ysp.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://sxr.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cvi.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lux.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xti.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://prm.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zai.daxiang520.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lbj.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jfn.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cir.hongshengwenyu.top

[D26] 数组转字符串
来源：http://odp.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://saz.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://inh.svipenyu.cn

JS:   arr.join(", ")
来源：http://fud.jinqigfzy.top

TS:   arr.join(", ")
来源：http://kim.daxiang520.top

Java: String.join(", ", list)
来源：http://mzl.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://epo.fzhhl.top

Ruby: arr.join(", ")
来源：http://fhx.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://opz.cucudq.cn

================================================================================
来源：http://tye.feifeiyinyue.top

E. 字符串处理
来源：http://yen.smart0.xyz

================================================================================
来源：http://hxy.sysykeji.top

[E01] 拼接字符串
来源：http://wby.yueranfly.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zbi.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xia.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dok.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jix.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://asd.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nfw.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aas.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://enj.ybcxt.top

[E02] 重复字符串
来源：http://cot.pengpengdd.cyou

Py:   "ab" * 3
来源：http://nvo.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://xyt.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://qch.yonumen.top

TS:   "ab".repeat(3)
来源：http://mzp.uphjek.com

Java: "ab".repeat(3)
来源：http://vbc.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://jyi.zhengqikj.top

Ruby: "ab" * 3
来源：http://mig.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cdp.sysykeji.top

[E03] 截取子串
来源：http://nau.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ekf.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tmf.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rzp.dashuyun.cn

TS:   s.slice(1, 4)
来源：http://ych.zdqjudy.top

Java: s.substring(1, 4)
来源：http://rnb.wangdashe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vww.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://adf.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://ivq.yangfankeji.com

[E04] 查找子串位置
来源：http://aej.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://tfb.wangdashe.top

PHP:  strpos($s, "x");
来源：http://ewj.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hvx.mhx1999.top

TS:   s.indexOf("x")
来源：http://kkp.yongpay.top

Java: s.indexOf("x")
来源：http://djh.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://jdi.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://jgl.fehbvm.com

C#:   s.IndexOf("x")
来源：http://fsh.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ued.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dlz.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ano.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rmm.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dok.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hpu.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cag.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ank.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://avm.tarul.cn

[E06] 替换子串
来源：http://iig.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uow.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://xmo.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://omi.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://zrz.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uhq.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://brr.cdnleiting.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xgw.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://wut.c1oappe.top

[E07] 按分隔符拆分
来源：http://eyc.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lox.shangyingyoupin.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ldn.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ckr.guannengcc.top

TS:   s.split(",")
来源：http://xmc.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jpf.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://igf.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://tkq.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://afu.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://yba.tarul.cn

Py:   ",".join(items)
来源：http://abb.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://zrr.ydjk.org.cn

JS:   items.join(",")
来源：http://xqv.zdbjq.cn

TS:   items.join(",")
来源：http://csx.fktsv.cn

Java: String.join(",", items)
来源：http://zmj.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://olc.hywenlv.cn

Ruby: items.join(",")
来源：http://kdq.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://mvc.tanke756.top

[E09] 去除所有空白字符
来源：http://gns.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mkg.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tfp.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://fhi.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://bie.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://mit.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yyx.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://ygu.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vvp.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://pgm.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hdz.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jla.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://dxw.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://uge.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://cuk.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ocv.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://twb.bjfxy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://klk.yj202588.top

[E11] 反转字符串
来源：http://zea.meibo888.top

Py:   s[::-1]
来源：http://irh.dashuyun.cn

PHP:  strrev($s);
来源：http://isd.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://wmz.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://emf.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://xpj.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eow.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://kwj.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://dpq.jinqigfzy.top

[E12] 统计某字符出现次数
来源：http://hza.hammf.cn

Py:   s.count("a")
来源：http://zfg.cheryme.top

PHP:  substr_count($s, "a");
来源：http://koq.epnwcf.com

JS:   s.split("a").length - 1
来源：http://fqt.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://bue.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://azr.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://pty.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://vwd.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://mtr.hnxiangtu.top

[E13] 逐字符遍历
来源：http://fyj.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://ffy.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jxv.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fng.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iiu.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://asa.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aoj.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ljl.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://grc.xuanzx.com

[E14] URL 编码与 Base64
来源：http://reg.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xth.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qqk.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://icu.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fwz.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vts.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pee.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://btx.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iyg.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://slx.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zld.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fbi.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xaa.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://avh.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lsm.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://brw.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sjv.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wsj.fengsongda.top

[E16] 数字千分位
来源：http://xaz.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://tja.yuanzhike.top

PHP:  number_format(1234567);
来源：http://obc.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oer.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cbv.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sje.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qqd.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bwa.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://hmi.zycfv.cn

[E17] 首字母大写
来源：http://oni.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://usp.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ihu.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wkj.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ehh.yvedp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wnz.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vvm.shangyingyoupin.top

Ruby: s.capitalize
来源：http://zmf.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iox.ppjwa.cn

[E18] 模板占位符替换
来源：http://uwm.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yyi.xingfuxueyuan.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lme.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yfc.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bcy.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xob.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xmd.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jfj.316326.xyz


<!-- 参考信息 -->