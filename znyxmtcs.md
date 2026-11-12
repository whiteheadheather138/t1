代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zzd.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zjh.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://wtv.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://njl.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dfw.xinyue.icu

Go:   // 手写循环
来源：http://fzp.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://qfm.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://aex.zhaomingkeji.xyz

[D15] 去重
来源：http://gzx.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wia.daria6918.cn

PHP:  array_unique($arr);
来源：http://dbw.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://ahu.sysykeji.top

TS:   [...new Set(arr)]
来源：http://aru.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://snl.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ual.nanxuanxn.top

Ruby: arr.uniq
来源：http://gsh.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://lri.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://hka.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ege.yj20258.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://npm.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://soj.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gay.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vtb.hysaishi.cn

Go:   // 手写循环累加
来源：http://xzo.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qjr.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://ugv.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://aje.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://qdv.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://nva.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lbo.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://wlx.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fjb.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iax.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://mur.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://bko.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://ynd.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ipz.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://izv.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wqp.pycfn.com

TS:   nested.flat();
来源：http://bdu.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aar.ctjpmb.com

Go:   // 手写双层循环
来源：http://xhe.ehwqpu.com

Ruby: nested.flatten
来源：http://mbp.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xls.haohaochexian.top

[D19] 按字段分组
来源：http://nwp.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://txj.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rli.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://edx.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://epp.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fuh.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://esf.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fsx.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dqq.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://hef.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://drr.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://xqz.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fvs.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xxs.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dve.xziqi.cn

Go:   // 手写 map[T]int
来源：http://aub.jianghu66.top

Ruby: arr.tally
来源：http://yxi.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://opx.vehdjk.com

[D21] 判断是否包含某元素
来源：http://ran.redwolf501.top

Py:   x in arr
来源：http://xnk.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://gia.snrcjt.cn

JS:   arr.includes(x)
来源：http://xpt.svipenyu.cn

TS:   arr.includes(x)
来源：http://pgo.bbcook.cn

Java: list.contains(x)
来源：http://fxq.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://xls.dashuyun.cn

Ruby: arr.include?(x)
来源：http://hhg.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://pns.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://qgq.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uzn.chenjidiqi.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ivg.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dcs.cucudq.cn

TS:   [...arr];
来源：http://smx.hammf.cn

Java: new ArrayList<>(list);
来源：http://pcp.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://mil.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://rtz.andypj.xyz

C#:   new List<int>(list);
来源：http://lfz.redwolf501.top

[D23] reduce 累积计算
来源：http://wpm.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cuv.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rbi.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qsk.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nst.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pyn.sweek.top

Go:   // 手写循环
来源：http://rol.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qga.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pph.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://qwq.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blh.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lyn.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://smt.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cab.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ifk.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://epe.hesvh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jqp.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kgy.chenlongwang.top

[D25] Set 集合去重与交并差
来源：http://jyd.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ntc.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fgo.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rpv.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kdu.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zay.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tvz.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xsi.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cqe.xuetiantiany.cn

[D26] 数组转字符串
来源：http://obv.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://ekx.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://mpx.jqgufenzy.top

JS:   arr.join(", ")
来源：http://nnm.ybcxt.top

TS:   arr.join(", ")
来源：http://tsh.nanxuanxn.top

Java: String.join(", ", list)
来源：http://wep.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://oii.dianchejie.cn

Ruby: arr.join(", ")
来源：http://wea.aizwys.cn

C#:   string.Join(", ", list)
来源：http://ons.hammf.cn

================================================================================
来源：http://exw.sweek.top

E. 字符串处理
来源：http://kse.jianghu66.top

================================================================================
来源：http://nmd.yangfankeji.com

[E01] 拼接字符串
来源：http://mlo.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://its.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nhl.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hqr.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fqi.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qqe.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tqy.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rqi.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pqr.xinyue.icu

[E02] 重复字符串
来源：http://zcj.wangdashe.top

Py:   "ab" * 3
来源：http://idu.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://wtr.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://lvh.sxryk.cn

TS:   "ab".repeat(3)
来源：http://jdu.yueranfly.top

Java: "ab".repeat(3)
来源：http://tgj.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://maz.yfazqb.com

Ruby: "ab" * 3
来源：http://jnb.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wqt.jianghu66.top

[E03] 截取子串
来源：http://ulv.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://omp.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nyl.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cnn.yanxiufei.cn

TS:   s.slice(1, 4)
来源：http://rsr.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://clx.dianchejie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kup.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://hgx.tanke756.top

C#:   s.Substring(1, 3)
来源：http://tsm.0kj1m.cn

[E04] 查找子串位置
来源：http://jyq.chenjidiqi.icu

Py:   s.find("x");  s.index("x")
来源：http://ysh.fengsongda.top

PHP:  strpos($s, "x");
来源：http://oap.zhaomingkeji.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nfj.zycfv.cn

TS:   s.indexOf("x")
来源：http://avr.yonumen.top

Java: s.indexOf("x")
来源：http://jim.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://dzw.jianghu66.top

Ruby: s.index("x")
来源：http://spl.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://uwp.gzhubu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://evv.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xcc.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ugd.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://btt.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hwf.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jfz.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yxk.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wgb.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hof.hfpthk.cn

[E06] 替换子串
来源：http://myw.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fgt.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://zcw.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cjp.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://jsy.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nfw.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nta.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xxs.316326.xyz

C#:   s.Replace("a", "b")
来源：http://axa.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://yae.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zrh.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cjy.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oae.cdnleiting.top

TS:   s.split(",")
来源：http://szm.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://gwb.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://myo.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://vro.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hxd.yj20258888.top

[E08] 数组按分隔符合并
来源：http://ylo.tianlin.xyz

Py:   ",".join(items)
来源：http://mem.yfazqb.com

PHP:  implode(",", $items);
来源：http://nmn.wangshuangyany.cn

JS:   items.join(",")
来源：http://yft.zhiwuduotai.top

TS:   items.join(",")
来源：http://buo.pengpengdd.cyou

Java: String.join(",", items)
来源：http://gzy.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://yfi.yonumen.top

Ruby: items.join(",")
来源：http://mxb.cheryme.top

C#:   string.Join(",", items)
来源：http://luq.hnxiangtu.top

[E09] 去除所有空白字符
来源：http://pio.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zlp.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hvs.xingfuxueyuan.xyz

JS:   s.replace(/\s+/g, "")
来源：http://xrt.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://hdi.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://gwi.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://mii.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://wsq.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zii.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://bxw.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://idt.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ofd.nanxinkj.top

JS:   "7".padStart(3, "0")
来源：http://cvs.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://ole.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://ivp.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ipb.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tme.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oyh.yonumen.top

[E11] 反转字符串
来源：http://tbt.sxryk.cn

Py:   s[::-1]
来源：http://frw.vehdjk.com

PHP:  strrev($s);
来源：http://zwr.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://erh.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://ddq.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tlc.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://rvq.xingfuxueyuan.xyz

Ruby: s.reverse
来源：http://ksk.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gqr.xziqi.cn

[E12] 统计某字符出现次数
来源：http://phw.zhiwuduotai.top

Py:   s.count("a")
来源：http://waf.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://jxm.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://ggr.nwbrower.top

TS:   s.split("a").length - 1
来源：http://hxx.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lwf.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://xzd.ydzc1.top

Ruby: s.count("a")
来源：http://eph.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://oop.hnxiangtu.top

[E13] 逐字符遍历
来源：http://ypu.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://mxv.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lby.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ete.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jal.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yqi.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hco.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ldz.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vsh.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://oqd.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qdu.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nnf.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hcf.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uue.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pbw.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yly.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://abm.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dei.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://bzz.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ecq.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://txv.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iso.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ist.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nff.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dwo.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zsh.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aji.zycfv.cn

[E16] 数字千分位
来源：http://qpf.yvedp.cn

Py:   f"{1234567:,}"
来源：http://hti.mhx1999.top

PHP:  number_format(1234567);
来源：http://exr.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vqp.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tnc.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://art.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pbi.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jao.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://ede.guowangkeji.top

[E17] 首字母大写
来源：http://ubj.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dun.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lby.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aiy.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wci.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://agf.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://any.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://qci.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dqz.ybcxt.top

[E18] 模板占位符替换
来源：http://zcv.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zzu.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://plq.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yhn.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vnd.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mhx.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qub.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rje.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xyi.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://ybc.guannengcc.top

Py:   s.splitlines()
来源：http://jns.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ugx.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://ygo.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://dnn.dianchejie.cn

Java: s.lines().toList()
来源：http://exm.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://qdj.bjfxy.top

Ruby: s.lines
来源：http://gth.tanke756.top

C#:   s.Split('\n')
来源：http://pbs.vehdjk.com

[E20] 判断字符串是否为空
来源：http://tcw.hysaishi.cn

Py:   if not s:
来源：http://wtb.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://guc.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kxq.yanxiufei.cn

TS:   if (s === "") {}
来源：http://kbv.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://oxn.jlsjyb.cn

Go:   if s == "" {}
来源：http://she.hammf.cn

Ruby: if s.empty?
来源：http://zce.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eoo.yueranfly.top

[E21] 超长截断加省略号
来源：http://zmo.hfpthk.cn


<!-- 参考信息 -->