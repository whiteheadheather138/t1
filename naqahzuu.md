代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xje.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://paw.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qnk.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://jon.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vqx.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xqh.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://juw.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://ufg.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fat.cucudq.cn

Go:   // 手写循环
来源：http://raw.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://rjw.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aen.ivvv.top

[D15] 去重
来源：http://klh.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eej.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://civ.aizwys.cn

JS:   [...new Set(arr)]
来源：http://xwf.yj20258.top

TS:   [...new Set(arr)]
来源：http://laq.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://enp.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tgu.nwbrower.top

Ruby: arr.uniq
来源：http://lco.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://ozr.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://nwk.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nta.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qej.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://crj.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gqr.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zyh.redwolf501.top

Go:   // 手写循环累加
来源：http://qur.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aza.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://gjz.xylfe.cn

[D17] 最大值与最小值
来源：http://ogq.tanke756.top

Py:   max(arr);  min(arr)
来源：http://vgb.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://ynv.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fwd.daxiang520.top

TS:   Math.max(...arr);
来源：http://mtz.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wcg.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://snm.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://ikm.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://qnd.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://xna.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nai.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://adq.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cjq.hnqzz.top

TS:   nested.flat();
来源：http://mlp.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vce.gotoacloud.top

Go:   // 手写双层循环
来源：http://ddn.jinqigufen.top

Ruby: nested.flatten
来源：http://fly.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tey.shzxlz.cn

[D19] 按字段分组
来源：http://dku.ydzc1.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qbl.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jqj.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nuv.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ski.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mhv.uphjek.com

Go:   // 手写 map[string][]T
来源：http://oid.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dzw.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jee.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://alf.pengpengdd.cyou

Py:   Counter(arr)
来源：http://yzs.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://rzt.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://plg.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wkl.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gav.iojbl.cn

Go:   // 手写 map[T]int
来源：http://wud.jianghu66.top

Ruby: arr.tally
来源：http://yxi.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yns.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://fhc.cucudq.cn

Py:   x in arr
来源：http://xad.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://gvn.yj202588.top

JS:   arr.includes(x)
来源：http://vbs.birdmap.top

TS:   arr.includes(x)
来源：http://kah.ehwqpu.com

Java: list.contains(x)
来源：http://dxy.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://dtz.vehdjk.com

Ruby: arr.include?(x)
来源：http://ccd.jqgfzy.top

C#:   list.Contains(x)
来源：http://yws.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://umj.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zqh.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://inv.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fag.yanxiufei.cn

TS:   [...arr];
来源：http://opv.sjlbkw.cn

Java: new ArrayList<>(list);
来源：http://aak.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://ybq.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://pei.bjfxy.top

C#:   new List<int>(list);
来源：http://oea.cashguo.top

[D23] reduce 累积计算
来源：http://zma.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bjy.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ogo.andypj.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://llj.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmd.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ydy.316326.xyz

Go:   // 手写循环
来源：http://jjq.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://itg.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oxn.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://wmb.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xwx.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nyb.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://imh.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iim.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vyz.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rrj.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lqr.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pgw.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://hqv.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hgl.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lse.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mof.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://grv.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dpi.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nht.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bbk.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xfe.9152youxi.cn

[D26] 数组转字符串
来源：http://lkt.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://uhi.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://bmk.tian-w.cn

JS:   arr.join(", ")
来源：http://qng.wangdashe.top

TS:   arr.join(", ")
来源：http://iex.fktsv.cn

Java: String.join(", ", list)
来源：http://hja.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://qrl.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://qgk.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://gxu.zhixingplan.top

================================================================================
来源：http://exu.nwbrower.top

E. 字符串处理
来源：http://mik.zhongyouzk.top

================================================================================
来源：http://hbu.c1oappe.top

[E01] 拼接字符串
来源：http://xqh.ydzc1.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://evd.hnxiangtu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://clp.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tbh.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxj.jqgfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vgf.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hzb.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://opx.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://igk.yj20258.top

[E02] 重复字符串
来源：http://bgt.hnxiangtu.top

Py:   "ab" * 3
来源：http://wle.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://hse.hammf.cn

JS:   "ab".repeat(3)
来源：http://fjv.fehbvm.com

TS:   "ab".repeat(3)
来源：http://sve.jiagoushi.top

Java: "ab".repeat(3)
来源：http://ddy.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://tdt.mhx1999.top

Ruby: "ab" * 3
来源：http://ogf.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hih.hysaishi.cn

[E03] 截取子串
来源：http://wbx.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gfi.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://khv.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dme.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://pph.daxiang520.top

Java: s.substring(1, 4)
来源：http://qhd.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fzn.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mpc.yonumen.top

C#:   s.Substring(1, 3)
来源：http://cim.yfazqb.com

[E04] 查找子串位置
来源：http://erc.yuxming.cn

Py:   s.find("x");  s.index("x")
来源：http://fzp.meibo888.top

PHP:  strpos($s, "x");
来源：http://khh.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kuo.cdnleiting.top

TS:   s.indexOf("x")
来源：http://vnf.sweek.top

Java: s.indexOf("x")
来源：http://llb.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://tvb.jlsjyb.cn

Ruby: s.index("x")
来源：http://qwk.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://htg.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hmh.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://elk.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jgj.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vvl.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ebr.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nhs.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uuk.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cqj.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xdq.cdnleiting.top

[E06] 替换子串
来源：http://tis.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vqh.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://vxy.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sgw.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://xzx.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ztv.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xwm.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://geb.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://wqc.pycfn.com

[E07] 按分隔符拆分
来源：http://ffi.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://byg.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://adt.yuxming.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://npy.cashguo.top

TS:   s.split(",")
来源：http://jib.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://wlu.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://orr.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://krv.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ynp.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://aiy.fktsv.cn

Py:   ",".join(items)
来源：http://mpl.cashguo.top

PHP:  implode(",", $items);
来源：http://saz.zhoulong.xyz

JS:   items.join(",")
来源：http://vpk.zhongyouzk.top

TS:   items.join(",")
来源：http://fdp.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://per.cheryme.top

Go:   strings.Join(items, ",")
来源：http://lol.hysaishi.cn

Ruby: items.join(",")
来源：http://lls.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://mhc.sufxvd.cn

[E09] 去除所有空白字符
来源：http://zmm.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eun.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://crp.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://dag.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://ahx.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://xrq.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kvq.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://krk.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ldt.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://aop.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://shx.nanxinkj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rwx.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://hgs.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://kbj.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://ylp.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vms.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qrt.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://umf.sjlbkw.cn

[E11] 反转字符串
来源：http://xox.aibaodan.cn

Py:   s[::-1]
来源：http://qko.wangdashe.top

PHP:  strrev($s);
来源：http://etg.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://moi.shangyingyoupin.top

TS:   [...s].reverse().join("")
来源：http://drk.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cte.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vaq.feifeiyinyue.top

Ruby: s.reverse
来源：http://fbn.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://kua.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://tps.c1oappe.top

Py:   s.count("a")
来源：http://vdq.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://gyx.yfazqb.com

JS:   s.split("a").length - 1
来源：http://cdt.cashguo.top

TS:   s.split("a").length - 1
来源：http://cbi.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nus.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://mmp.redwolf501.top

Ruby: s.count("a")
来源：http://vua.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://fwk.xylfe.cn

[E13] 逐字符遍历
来源：http://gtr.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://uks.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hno.mhx1999.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gve.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dhk.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tzy.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sgg.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://frr.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wwl.shanyushiyangkeji.top

[E14] URL 编码与 Base64
来源：http://voh.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xcz.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pbg.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ovd.0kj1m.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xje.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yzd.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://usl.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xlf.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gca.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://xpm.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vez.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qrp.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sdk.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jvh.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ghh.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lyw.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yhj.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zjf.yonumen.top

[E16] 数字千分位
来源：http://ama.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://uvz.52xcode.cn

PHP:  number_format(1234567);
来源：http://xkp.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://cnq.jinyuanbaomall.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qof.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vpi.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zvh.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bim.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://zjy.pengpengdd.cyou

[E17] 首字母大写
来源：http://ejg.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jhy.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yjb.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pko.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eil.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dxa.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mvv.ydzc1.top

Ruby: s.capitalize
来源：http://dre.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fvf.hcnkem.com

[E18] 模板占位符替换
来源：http://glz.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uiz.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zft.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cbd.jyoumei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zjc.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dul.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qur.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xit.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://miv.yueranfly.top

[E19] 多行文本按行拆分
来源：http://hif.52xcode.cn

Py:   s.splitlines()
来源：http://zwl.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rzy.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://dth.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://vej.birdmap.top

Java: s.lines().toList()
来源：http://xdw.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://ixs.xuetiantiany.cn

Ruby: s.lines
来源：http://kbd.pycfn.com

C#:   s.Split('\n')
来源：http://ocp.yj20258.top

[E20] 判断字符串是否为空
来源：http://vbb.ctjpmb.com

Py:   if not s:
来源：http://gbv.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gbb.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lao.jqgufenzy.top

TS:   if (s === "") {}
来源：http://mxe.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://wfw.hnqzz.top


<!-- 参考信息 -->