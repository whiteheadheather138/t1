代发 wailian999

TS:   [...new Set(arr)]
来源：http://zib.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hax.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://tjz.tianlin.xyz

Ruby: arr.uniq
来源：http://hwh.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://wep.nanxinkj.top

[D16] 求和与平均值
来源：http://geh.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hjk.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tvo.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bot.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dbn.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pps.ehwqpu.com

Go:   // 手写循环累加
来源：http://jma.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://prb.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://tms.cashguo.top

[D17] 最大值与最小值
来源：http://bun.nanxinkj.top

Py:   max(arr);  min(arr)
来源：http://bul.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://vtj.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jtz.xuanzx.com

TS:   Math.max(...arr);
来源：http://iyu.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://nxh.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lju.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://gik.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://ucv.tarul.cn

[D18] 扁平化嵌套数组
来源：http://znx.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lso.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://dth.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iir.ehwqpu.com

TS:   nested.flat();
来源：http://cwl.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lxc.mhx1999.top

Go:   // 手写双层循环
来源：http://kgs.sxryk.cn

Ruby: nested.flatten
来源：http://irn.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wuv.daxiang520.top

[D19] 按字段分组
来源：http://pbi.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uwd.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xhp.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uom.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kmp.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yza.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://wkq.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xie.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://spg.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://hxd.zhixingplan.top

Py:   Counter(arr)
来源：http://hzn.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://ycf.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lqa.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uzr.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dur.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://kjf.aizwys.cn

Ruby: arr.tally
来源：http://kbo.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ofk.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://sxd.iojbl.cn

Py:   x in arr
来源：http://fgl.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://hnt.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://hfv.smart0.xyz

TS:   arr.includes(x)
来源：http://ara.fengsongda.top

Java: list.contains(x)
来源：http://epi.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://jzc.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://qlw.fehbvm.com

C#:   list.Contains(x)
来源：http://ehq.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://szu.ybcxt.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zfj.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tga.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://epb.xylfe.cn

TS:   [...arr];
来源：http://yvz.tanke756.top

Java: new ArrayList<>(list);
来源：http://job.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://lbo.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://fpe.snrcjt.cn

C#:   new List<int>(list);
来源：http://fuh.ctjpmb.com

[D23] reduce 累积计算
来源：http://kxf.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zwy.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pao.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyp.cashguo.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nkr.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://rcp.zhiwuduotai.top

Go:   // 手写循环
来源：http://lms.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ita.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://meh.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://jcq.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kov.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tju.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kue.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nms.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kwb.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://drm.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uba.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cdm.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://sys.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://khe.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sen.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xjw.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://usw.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://txq.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lbz.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aqj.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mbp.gzhubu.top

[D26] 数组转字符串
来源：http://qqg.mhx1999.top

Py:   ", ".join(map(str, arr))
来源：http://yqk.havefunace.top

PHP:  implode(", ", $arr);
来源：http://mub.gotoacloud.top

JS:   arr.join(", ")
来源：http://nnw.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://mkz.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://ckx.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://whl.ehwqpu.com

Ruby: arr.join(", ")
来源：http://mnt.uphjek.com

C#:   string.Join(", ", list)
来源：http://wqq.wangshuangyany.cn

================================================================================
来源：http://umt.pengpengdd.cyou

E. 字符串处理
来源：http://oos.havefunace.top

================================================================================
来源：http://eat.yj202588.top

[E01] 拼接字符串
来源：http://vkm.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ohq.guowangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tqu.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://obt.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lyx.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ekd.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dwk.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dpc.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oax.yj20258.top

[E02] 重复字符串
来源：http://nfr.andypj.xyz

Py:   "ab" * 3
来源：http://esd.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://fov.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://tho.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://mgs.sufxvd.cn

Java: "ab".repeat(3)
来源：http://lvt.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://poa.zhoulong.xyz

Ruby: "ab" * 3
来源：http://dth.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://drk.jianghu66.top

[E03] 截取子串
来源：http://qdf.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://krw.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://veb.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cqk.hesvh.cn

TS:   s.slice(1, 4)
来源：http://nux.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://kre.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://arm.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://zvs.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://lfo.feifeiyinyue.top

[E04] 查找子串位置
来源：http://hub.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://prc.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://mui.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lls.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://nhq.xylfe.cn

Java: s.indexOf("x")
来源：http://afc.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://cyq.cqqwz.cn

Ruby: s.index("x")
来源：http://gky.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://wvh.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vyu.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rko.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://riz.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rke.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vur.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xmz.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uyw.hnqzz.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lyb.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wsm.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://crt.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://glu.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://ziu.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wtg.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://gri.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://frj.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gft.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wzv.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://dlu.svipenyu.cn

[E07] 按分隔符拆分
来源：http://ysw.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cth.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vqz.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://noi.fanxiaobao.xyz

TS:   s.split(",")
来源：http://wmu.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://rrl.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lhz.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://tin.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yfj.vehdjk.com

[E08] 数组按分隔符合并
来源：http://uys.aibaodan.cn

Py:   ",".join(items)
来源：http://hrr.zhixingplan.top

PHP:  implode(",", $items);
来源：http://pdj.yuanzhike.top

JS:   items.join(",")
来源：http://mhq.nwbrower.top

TS:   items.join(",")
来源：http://eig.svipenyu.cn

Java: String.join(",", items)
来源：http://gcd.shuidangran.top

Go:   strings.Join(items, ",")
来源：http://ogk.hnxiangtu.top

Ruby: items.join(",")
来源：http://zxl.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://way.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://ljg.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oyf.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hdr.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://zar.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://cic.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://pjy.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mir.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jgg.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cly.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://kzo.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dlf.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://znc.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://vgd.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://cwd.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://wfe.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gqe.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jik.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://djx.pycfn.com

[E11] 反转字符串
来源：http://klh.wangshuangyany.cn

Py:   s[::-1]
来源：http://ffp.jiagoushi.top

PHP:  strrev($s);
来源：http://kwu.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://rnb.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://uqt.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://npk.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://yyi.xuanzx.com

Ruby: s.reverse
来源：http://yqw.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://rji.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://yjq.fanxiaobao.xyz

Py:   s.count("a")
来源：http://uss.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://xdd.hammf.cn

JS:   s.split("a").length - 1
来源：http://kng.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://ada.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://juq.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://wkr.sysykeji.top

Ruby: s.count("a")
来源：http://lnv.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://afa.daria6918.cn

[E13] 逐字符遍历
来源：http://whj.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://dhy.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cwu.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rbu.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pjk.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jbt.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pnn.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wgm.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sju.pycfn.com

[E14] URL 编码与 Base64
来源：http://sgf.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hme.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dfk.shanyushiyangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uel.bjfxy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hal.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vul.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mtw.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yhm.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://izl.shanyushiyangtech.top

[E15] HTML 转义 / 反转义
来源：http://pbt.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nwp.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ngi.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tyj.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ezj.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bzs.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lyl.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://shu.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nxb.ybcxt.top

[E16] 数字千分位
来源：http://bjb.meibo888.top

Py:   f"{1234567:,}"
来源：http://hnt.cheryme.top

PHP:  number_format(1234567);
来源：http://uhg.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rek.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zsi.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sjw.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vye.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kyb.tarul.cn

C#:   1234567.ToString("N0")
来源：http://buj.yvedp.cn

[E17] 首字母大写
来源：http://wkk.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://auu.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xxa.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://weh.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mxh.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zxl.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gyh.fehbvm.com

Ruby: s.capitalize
来源：http://psc.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gvu.yuxming.cn

[E18] 模板占位符替换
来源：http://ulg.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://emy.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kgu.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://mxe.shanyushiyangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zcm.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://quz.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bnz.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://clb.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yec.daria6918.cn

[E19] 多行文本按行拆分
来源：http://vka.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://ktf.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://obo.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://hoy.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://jcl.gotoacloud.top

Java: s.lines().toList()
来源：http://guj.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://ifc.uphjek.com

Ruby: s.lines
来源：http://rlu.mhx1999.top

C#:   s.Split('\n')
来源：http://fae.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://sim.52xcode.cn

Py:   if not s:
来源：http://cox.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ddb.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ahs.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://grq.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://eab.tian-w.cn

Go:   if s == "" {}
来源：http://kzc.pengpengdd.cyou

Ruby: if s.empty?
来源：http://vcj.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gjf.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://zlm.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zfw.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xzx.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://skv.shzxlz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gug.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ovg.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://hvz.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gcj.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xgv.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://yxu.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qhl.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pxr.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hbq.hesvh.cn


<!-- 参考信息 -->