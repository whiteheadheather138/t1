代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hlz.chenzaomai.com

[D16] 求和与平均值
来源：http://xgn.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://prh.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nfl.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://krd.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ulv.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uje.quarkkingdee.top

Go:   // 手写循环累加
来源：http://ryd.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hbv.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://ivm.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://iaw.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://yfw.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://fqk.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pls.daria6918.cn

TS:   Math.max(...arr);
来源：http://qqd.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bso.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tev.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://hjy.chenjidiqi.icu

C#:   list.Max();  list.Min()
来源：http://maq.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://cqu.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pkl.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://qxz.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uer.dashuyun.cn

TS:   nested.flat();
来源：http://fut.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tot.jinqigfzy.top

Go:   // 手写双层循环
来源：http://xkv.dianchejie.cn

Ruby: nested.flatten
来源：http://rxg.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wce.dashuyun.cn

[D19] 按字段分组
来源：http://kbi.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uby.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://frh.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nmr.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://zra.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://een.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://ifr.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jdp.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kud.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://byt.fehbvm.com

Py:   Counter(arr)
来源：http://rwz.yangfankeji.com

PHP:  array_count_values($arr);
来源：http://upc.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mzt.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ngn.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://btz.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://aia.gotoacloud.top

Ruby: arr.tally
来源：http://wam.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eak.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://asp.52xcode.cn

Py:   x in arr
来源：http://brk.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://rsq.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://nfl.cheryme.top

TS:   arr.includes(x)
来源：http://cla.andypj.xyz

Java: list.contains(x)
来源：http://sgt.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://uok.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://smw.vehdjk.com

C#:   list.Contains(x)
来源：http://zyt.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://qjd.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xqg.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lzg.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xra.tanke756.top

TS:   [...arr];
来源：http://lon.havefunace.top

Java: new ArrayList<>(list);
来源：http://xzh.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dib.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://nzc.chenzaomai.com

C#:   new List<int>(list);
来源：http://wep.nwbrower.top

[D23] reduce 累积计算
来源：http://rao.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hey.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cma.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bqt.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://szs.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iqb.pengpengdd.cyou

Go:   // 手写循环
来源：http://ubg.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://whz.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jex.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://akm.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gbn.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mtf.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ecy.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rzn.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ncy.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://laa.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qec.gotoacloud.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cnf.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://lty.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xvh.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dzg.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rir.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dck.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sju.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jub.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xjd.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tgj.xziqi.cn

[D26] 数组转字符串
来源：http://oel.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://kyq.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://drl.haohaochexian.top

JS:   arr.join(", ")
来源：http://jvj.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://qls.jqgfzy.top

Java: String.join(", ", list)
来源：http://ltn.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://xkw.sufxvd.cn

Ruby: arr.join(", ")
来源：http://jiy.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://lgs.jqgfzy.top

================================================================================
来源：http://jdc.mhx1999.top

E. 字符串处理
来源：http://kxk.chenjidiqi.icu

================================================================================
来源：http://eus.xinyue.icu

[E01] 拼接字符串
来源：http://efz.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://svj.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nuc.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pwa.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vsu.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fyp.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xvl.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://crm.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://azs.hysaishi.cn

[E02] 重复字符串
来源：http://gjm.yuxming.cn

Py:   "ab" * 3
来源：http://kym.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://cov.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://rqo.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://eop.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://rff.jiagoushi.top

Go:   strings.Repeat("ab", 3)
来源：http://ydv.nwbrower.top

Ruby: "ab" * 3
来源：http://gfn.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bot.jlsjyb.cn

[E03] 截取子串
来源：http://zrz.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wrv.sysykeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ypn.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tcq.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://xov.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://kcr.dianchejie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hvi.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lpf.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://nlp.yfazqb.com

[E04] 查找子串位置
来源：http://qzi.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://qdc.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://ttr.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zvo.shzxlz.cn

TS:   s.indexOf("x")
来源：http://fod.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://htv.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://xtj.nanxuanxn.top

Ruby: s.index("x")
来源：http://pte.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://unz.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tei.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bca.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dxl.cheryme.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jtu.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pah.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lkz.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tdg.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xvr.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rro.yuxming.cn

[E06] 替换子串
来源：http://knm.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ygq.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://fut.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vfz.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://dqz.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nio.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wwb.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lfn.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://bnj.birdmap.top

[E07] 按分隔符拆分
来源：http://rkz.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ajm.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ypi.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ykl.yuxming.cn

TS:   s.split(",")
来源：http://krw.svipenyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dph.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dja.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://mmb.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mgd.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://tre.ydzc1.top

Py:   ",".join(items)
来源：http://jmf.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://iqo.jiagoushi.top

JS:   items.join(",")
来源：http://upr.yfazqb.com

TS:   items.join(",")
来源：http://gww.316326.xyz

Java: String.join(",", items)
来源：http://uuq.havefunace.top

Go:   strings.Join(items, ",")
来源：http://plt.snrcjt.cn

Ruby: items.join(",")
来源：http://ucw.jinqigufen.top

C#:   string.Join(",", items)
来源：http://lin.daria6918.cn

[E09] 去除所有空白字符
来源：http://bfw.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tlz.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gdf.nanxuanxn.top

JS:   s.replace(/\s+/g, "")
来源：http://kdp.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://zms.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://qrb.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qzp.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://nzr.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ivb.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://jxk.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fry.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vfl.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://asu.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://ljt.aizwys.cn

Java: String.format("%03d", 7)
来源：http://fgh.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://psv.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mbm.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ppk.chenzaomai.com

[E11] 反转字符串
来源：http://ypx.pengpengdd.cyou

Py:   s[::-1]
来源：http://ard.svipenyu.cn

PHP:  strrev($s);
来源：http://doy.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://fyb.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://zaw.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://exs.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sgp.ppjwa.cn

Ruby: s.reverse
来源：http://gvt.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://qmi.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://vvz.vehdjk.com

Py:   s.count("a")
来源：http://dov.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://yeq.mhx1999.top

JS:   s.split("a").length - 1
来源：http://llk.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://mvf.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qeo.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://gkg.aizwys.cn

Ruby: s.count("a")
来源：http://vbx.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://rwe.cashguo.top

[E13] 逐字符遍历
来源：http://vqj.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://hzc.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xrd.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fwv.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://enu.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yva.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://glm.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://evs.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vxb.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://hoq.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zue.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rsz.vqdsnc.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jbj.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iwp.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zen.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kdq.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://juo.cdnleiting.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yai.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://zri.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tgx.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fgf.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://art.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ilm.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zfx.sufxvd.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lhv.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://swm.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nwe.hammf.cn

[E16] 数字千分位
来源：http://ouw.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://tdk.jinqigufen.top

PHP:  number_format(1234567);
来源：http://enc.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://piy.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zkw.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rzx.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wcd.ywan-chungtsiang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pyp.pycfn.com

C#:   1234567.ToString("N0")
来源：http://neb.jqgfzy.top

[E17] 首字母大写
来源：http://lyn.ydjk.org.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cgd.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gnt.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nzd.jinqigfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sbl.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pjy.c1oappe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rps.cdnleiting.top

Ruby: s.capitalize
来源：http://iri.yj202588.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xac.yuanzhike.top

[E18] 模板占位符替换
来源：http://hsb.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tpx.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xhq.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cbj.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://prt.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://axn.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oyq.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fsb.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://psi.jianghu66.top

[E19] 多行文本按行拆分
来源：http://zfd.aizwys.cn

Py:   s.splitlines()
来源：http://afd.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://klk.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://arg.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://qqc.iojbl.cn

Java: s.lines().toList()
来源：http://lxk.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://pzv.snrcjt.cn

Ruby: s.lines
来源：http://vdz.aizwys.cn

C#:   s.Split('\n')
来源：http://gnd.yongpay.top

[E20] 判断字符串是否为空
来源：http://fre.mhx1999.top

Py:   if not s:
来源：http://nfc.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zom.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ozp.yanxiufei.cn

TS:   if (s === "") {}
来源：http://wmd.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://sby.pengpengdd.cyou

Go:   if s == "" {}
来源：http://ylp.jinqigufen.top

Ruby: if s.empty?
来源：http://pxh.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ann.hesvh.cn

[E21] 超长截断加省略号
来源：http://hjk.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://epa.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hhw.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://acl.jiagoushi.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pfw.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cmc.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://xxd.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oet.hywenlv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ylc.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://qzp.zdbjq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pao.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kla.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gum.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lko.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ysb.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jde.yfazqb.com

Ruby: s.bytesize;  s.length
来源：http://uuc.sysykeji.top


<!-- 参考信息 -->