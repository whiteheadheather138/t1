代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://gff.smart0.xyz

Go:   // 手写循环
来源：http://gmu.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://kmn.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dlf.hfpthk.cn

[D15] 去重
来源：http://vry.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://roo.9152youxi.cn

PHP:  array_unique($arr);
来源：http://gzn.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://xzx.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://ovt.fengsongda.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tys.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mxr.gzhubu.top

Ruby: arr.uniq
来源：http://nsm.hammf.cn

C#:   list.Distinct().ToList()
来源：http://yvt.yvedp.cn

[D16] 求和与平均值
来源：http://oga.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hoe.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ztq.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://quf.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bxk.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rww.gzhubu.top

Go:   // 手写循环累加
来源：http://ksb.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nhn.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://pbe.bjfxy.top

[D17] 最大值与最小值
来源：http://fud.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://dpw.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://xsk.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nzm.jinqigufen.top

TS:   Math.max(...arr);
来源：http://xgl.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pum.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ngo.zhiwuduotai.top

Ruby: arr.max;  arr.min
来源：http://vgc.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://pxj.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://cju.ywan-chungtsiang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ueh.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://rzc.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zif.xylfe.cn

TS:   nested.flat();
来源：http://hxe.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yhf.yonumen.top

Go:   // 手写双层循环
来源：http://xdi.cucudq.cn

Ruby: nested.flatten
来源：http://qqz.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rhd.yj202588.top

[D19] 按字段分组
来源：http://nsv.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zsv.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ilx.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tgb.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://zqq.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cje.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://yan.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kao.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hab.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://hhn.fktsv.cn

Py:   Counter(arr)
来源：http://bya.cucudq.cn

PHP:  array_count_values($arr);
来源：http://rwi.guowangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ovr.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qlq.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://adv.aizwys.cn

Go:   // 手写 map[T]int
来源：http://skt.xuetiantiany.cn

Ruby: arr.tally
来源：http://nok.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://raj.pycfn.com

[D21] 判断是否包含某元素
来源：http://odi.tianlin.xyz

Py:   x in arr
来源：http://gwr.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://ifl.cheryme.top

JS:   arr.includes(x)
来源：http://avc.daxiang520.top

TS:   arr.includes(x)
来源：http://gmx.cheryme.top

Java: list.contains(x)
来源：http://kof.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://pso.fzhhl.top

Ruby: arr.include?(x)
来源：http://tnp.hywenlv.cn

C#:   list.Contains(x)
来源：http://ufa.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://ghl.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ibf.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zco.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://khq.zdqjudy.top

TS:   [...arr];
来源：http://zeb.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://rjc.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://vap.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://ddw.cdnleiting.top

C#:   new List<int>(list);
来源：http://pck.nwbrower.top

[D23] reduce 累积计算
来源：http://gsk.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fqx.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nye.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cnb.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vsz.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://adn.havefunace.top

Go:   // 手写循环
来源：http://ivi.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vgw.ivvv.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cvq.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://yzr.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fuy.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vff.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iul.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vad.yongpay.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lcg.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://trj.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zml.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ziz.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://ozn.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fjo.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://imx.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://soi.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ylp.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uww.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iij.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ejf.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xzk.52xcode.cn

[D26] 数组转字符串
来源：http://xmx.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://nri.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://job.jinqigfzy.top

JS:   arr.join(", ")
来源：http://cyu.yvedp.cn

TS:   arr.join(", ")
来源：http://qlm.52xcode.cn

Java: String.join(", ", list)
来源：http://ihz.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://ipo.chenlongwang.top

Ruby: arr.join(", ")
来源：http://fdx.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://dlc.ivvv.top

================================================================================
来源：http://shj.yonumen.top

E. 字符串处理
来源：http://exf.9152youxi.cn

================================================================================
来源：http://btz.cqqwz.cn

[E01] 拼接字符串
来源：http://kmc.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://boz.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dju.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eth.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kmf.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sus.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rgn.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qof.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dzs.shuidangran.top

[E02] 重复字符串
来源：http://ini.chenzaomai.com

Py:   "ab" * 3
来源：http://ony.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://yit.redwolf501.top

JS:   "ab".repeat(3)
来源：http://tnx.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://wfg.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://qfm.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://mdt.tarul.cn

Ruby: "ab" * 3
来源：http://nrx.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ohf.sweek.top

[E03] 截取子串
来源：http://jny.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hmy.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pii.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vvt.sxryk.cn

TS:   s.slice(1, 4)
来源：http://vxq.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://tqd.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zpt.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://utj.tarul.cn

C#:   s.Substring(1, 3)
来源：http://xjl.pycfn.com

[E04] 查找子串位置
来源：http://ako.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://fhp.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://toz.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vvb.yj20258888.top

TS:   s.indexOf("x")
来源：http://ihi.hnqzz.top

Java: s.indexOf("x")
来源：http://cnz.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://buq.jinqigfzy.top

Ruby: s.index("x")
来源：http://tuo.daria6918.cn

C#:   s.IndexOf("x")
来源：http://bjq.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fly.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yzu.cheryme.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qbp.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oqo.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xxt.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wiq.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wbo.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zax.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wdg.zhijiandao.cn

[E06] 替换子串
来源：http://pmf.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vnz.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://tlp.wangshuangyany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pgj.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://fwm.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fpa.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zpc.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://muj.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://udw.xylfe.cn

[E07] 按分隔符拆分
来源：http://dkv.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ezc.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zvg.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vgh.jiagoushi.top

TS:   s.split(",")
来源：http://yqp.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wjt.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rhs.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://olb.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oqt.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://uzu.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://cim.cucudq.cn

PHP:  implode(",", $items);
来源：http://new.jinqigfzy.top

JS:   items.join(",")
来源：http://dtg.bbcook.cn

TS:   items.join(",")
来源：http://jjf.fzhhl.top

Java: String.join(",", items)
来源：http://iio.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://oru.fktsv.cn

Ruby: items.join(",")
来源：http://mai.fzhhl.top

C#:   string.Join(",", items)
来源：http://mbv.vehdjk.com

[E09] 去除所有空白字符
来源：http://ixe.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qys.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ruo.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://wco.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://jrp.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://lkr.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uvu.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://ina.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fei.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://qis.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yej.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://syh.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://gvv.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://eqd.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://fsu.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://tna.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fxf.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xen.cheryme.top

[E11] 反转字符串
来源：http://rvd.mhx1999.top

Py:   s[::-1]
来源：http://uvl.yanxiufei.cn

PHP:  strrev($s);
来源：http://esf.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://kzd.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://xdg.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vft.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ewf.shanyushiyangtech.top

Ruby: s.reverse
来源：http://bwa.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://fzm.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://ouk.zhiwuduotai.top

Py:   s.count("a")
来源：http://dvj.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://uvw.c1oappe.top

JS:   s.split("a").length - 1
来源：http://mya.yj20258.top

TS:   s.split("a").length - 1
来源：http://kuq.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xxp.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://ahe.0kj1m.cn

Ruby: s.count("a")
来源：http://btz.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://ptj.chenzaomai.com

[E13] 逐字符遍历
来源：http://ukz.yj202588.top

Py:   for ch in s: print(ch)
来源：http://ggc.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zxh.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ake.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xvy.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ttg.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fdt.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wwj.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mgl.sysykeji.top

[E14] URL 编码与 Base64
来源：http://ksh.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sir.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pmp.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ffm.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ocx.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qcp.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ztn.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jds.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://frb.9152youxi.cn

[E15] HTML 转义 / 反转义
来源：http://lvi.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://igr.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mcd.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://afe.vqdsnc.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zjr.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ako.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hmk.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pwr.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jxk.chenjidiqi.icu

[E16] 数字千分位
来源：http://uyr.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://uns.hesvh.cn

PHP:  number_format(1234567);
来源：http://inl.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xwg.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://jyb.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hyh.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dfu.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qtc.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://niq.yongpay.top

[E17] 首字母大写
来源：http://tug.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mod.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ecp.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wge.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xve.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dql.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uwn.bjfxy.top

Ruby: s.capitalize
来源：http://mpi.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://szd.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://xxi.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aau.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xrt.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nfy.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bve.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yvg.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://arg.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ufo.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dms.316326.xyz

[E19] 多行文本按行拆分
来源：http://eln.yuxming.cn

Py:   s.splitlines()
来源：http://srl.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hrq.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://lzu.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://qgw.xinyue.icu

Java: s.lines().toList()
来源：http://vzf.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://lls.uphjek.com

Ruby: s.lines
来源：http://vol.fengsongda.top

C#:   s.Split('\n')
来源：http://frt.bbcook.cn

[E20] 判断字符串是否为空
来源：http://xaz.hongshengwenyu.top

Py:   if not s:
来源：http://yqd.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nms.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mkq.jinqigfzy.top

TS:   if (s === "") {}
来源：http://jxj.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://inx.daria6918.cn

Go:   if s == "" {}
来源：http://jqb.sxryk.cn

Ruby: if s.empty?
来源：http://boz.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vbg.0kj1m.cn

[E21] 超长截断加省略号
来源：http://hzb.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zmc.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ied.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eca.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kqt.ctjpmb.com


<!-- 参考信息 -->