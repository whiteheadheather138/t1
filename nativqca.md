代发 wailian999

C#:   list.Distinct().ToList()
来源：http://ukw.hcnkem.com

[D16] 求和与平均值
来源：http://qeg.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mnq.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://for.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gir.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vey.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://enm.fktsv.cn

Go:   // 手写循环累加
来源：http://dux.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jvo.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://vkn.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://qpr.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://pta.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://cvd.zdbjq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oet.gzhubu.top

TS:   Math.max(...arr);
来源：http://krg.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eey.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://got.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://fqz.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://eko.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://iye.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dnt.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://xrl.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gsd.zhongyouzk.top

TS:   nested.flat();
来源：http://jzo.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qcq.shuidangran.top

Go:   // 手写双层循环
来源：http://jdl.ydzc1.top

Ruby: nested.flatten
来源：http://xsp.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xot.zdqjudy.top

[D19] 按字段分组
来源：http://gcq.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://orz.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dud.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://asm.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nub.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gvk.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://sst.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://czk.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yyg.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://yzd.guowangkeji.top

Py:   Counter(arr)
来源：http://lvp.cucudq.cn

PHP:  array_count_values($arr);
来源：http://xnn.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qnm.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aaj.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xug.hesvh.cn

Go:   // 手写 map[T]int
来源：http://rkm.hywenlv.cn

Ruby: arr.tally
来源：http://rrq.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mhn.tarul.cn

[D21] 判断是否包含某元素
来源：http://vfx.havefunace.top

Py:   x in arr
来源：http://qey.quarkkingdee.top

PHP:  in_array($x, $arr, true);
来源：http://ssr.gzhubu.top

JS:   arr.includes(x)
来源：http://rfk.yvedp.cn

TS:   arr.includes(x)
来源：http://eiy.yanxiufei.cn

Java: list.contains(x)
来源：http://tgf.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://bqs.fktsv.cn

Ruby: arr.include?(x)
来源：http://lya.zycfv.cn

C#:   list.Contains(x)
来源：http://ewj.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://jnd.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tzz.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qae.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nte.gogol.net.cn

TS:   [...arr];
来源：http://prv.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://dxi.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gkn.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://sao.gotoacloud.top

C#:   new List<int>(list);
来源：http://ttm.hysaishi.cn

[D23] reduce 累积计算
来源：http://slu.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mpj.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rql.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kym.ydzc1.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ztw.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oic.ydjk.org.cn

Go:   // 手写循环
来源：http://tym.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qjn.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tcj.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://pja.gaohongyu789.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rzd.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wrs.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pus.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bmm.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iaj.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fqk.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nmn.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wqc.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://vpr.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kje.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aov.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qos.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fxj.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jgn.jlsjyb.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uzg.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hki.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ryn.sjlbkw.cn

[D26] 数组转字符串
来源：http://yms.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://gdk.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://elp.gogol.net.cn

JS:   arr.join(", ")
来源：http://equ.vehdjk.com

TS:   arr.join(", ")
来源：http://qiy.jqgufenzy.top

Java: String.join(", ", list)
来源：http://mel.jianghu66.top

Go:   strings.Join(strs, ", ")
来源：http://kxj.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://oft.ybcxt.top

C#:   string.Join(", ", list)
来源：http://yof.hongshengwenyu.top

================================================================================
来源：http://ozx.ivvv.top

E. 字符串处理
来源：http://yng.tanke756.top

================================================================================
来源：http://lyp.haohaochexian.top

[E01] 拼接字符串
来源：http://qcb.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vas.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://imq.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tjl.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://swc.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ydy.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ycj.sjlbkw.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://unr.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jdm.tianlin.xyz

[E02] 重复字符串
来源：http://zki.ydzc1.top

Py:   "ab" * 3
来源：http://hxm.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://zwj.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://zvf.yj202588.top

TS:   "ab".repeat(3)
来源：http://qjj.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://udq.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://nys.haohaochexian.top

Ruby: "ab" * 3
来源：http://luy.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qau.dianchejie.cn

[E03] 截取子串
来源：http://zke.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qqr.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://njf.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rsu.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://frp.chenlongwang.top

Java: s.substring(1, 4)
来源：http://txh.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fuv.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fei.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://pbj.haohaochexian.top

[E04] 查找子串位置
来源：http://lzh.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://rtj.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://xwf.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gtu.hfpthk.cn

TS:   s.indexOf("x")
来源：http://oaa.yj20258888.top

Java: s.indexOf("x")
来源：http://nha.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://ibc.yj20258.top

Ruby: s.index("x")
来源：http://sqm.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://mzd.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zii.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lmy.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://skf.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oqf.xuanzx.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://uov.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pnh.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ogb.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lic.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mex.sufxvd.cn

[E06] 替换子串
来源：http://owe.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gow.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://eud.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ftu.birdmap.top

TS:   s.replaceAll("a", "b")
来源：http://rzd.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://urz.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://huy.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jfl.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://icu.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://hxg.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nuu.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://btn.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://asn.yueranfly.top

TS:   s.split(",")
来源：http://sec.gzhubu.top

Java: s.split(",");  s.split("\\s+")
来源：http://rvd.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vzq.haohaochexian.top

Ruby: s.split(",");  s.split
来源：http://bdd.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vhq.andypj.xyz

[E08] 数组按分隔符合并
来源：http://edx.bbcook.cn

Py:   ",".join(items)
来源：http://ssa.ppjwa.cn

PHP:  implode(",", $items);
来源：http://yzw.xylfe.cn

JS:   items.join(",")
来源：http://mix.fengsongda.top

TS:   items.join(",")
来源：http://udm.gotoacloud.top

Java: String.join(",", items)
来源：http://lnd.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://ypi.snrcjt.cn

Ruby: items.join(",")
来源：http://nhe.tianlin.xyz

C#:   string.Join(",", items)
来源：http://mvh.gogol.net.cn

[E09] 去除所有空白字符
来源：http://dfj.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blt.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eda.yuanzhike.top

JS:   s.replace(/\s+/g, "")
来源：http://wno.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://gfi.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://rdj.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ahq.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://zqh.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://twn.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://rsi.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aox.ivvv.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iev.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://zmr.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://uje.bjfxy.top

Java: String.format("%03d", 7)
来源：http://bcj.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://myv.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sbj.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cao.zdqjudy.top

[E11] 反转字符串
来源：http://mcl.snrcjt.cn

Py:   s[::-1]
来源：http://wkw.tian-w.cn

PHP:  strrev($s);
来源：http://neo.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://qlc.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://loz.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qap.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jtn.hnxiangtu.top

Ruby: s.reverse
来源：http://htn.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://prf.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://cfm.aizwys.cn

Py:   s.count("a")
来源：http://ccn.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://epq.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://lyv.yvedp.cn

TS:   s.split("a").length - 1
来源：http://uit.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://guc.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://byb.guannengcc.top

Ruby: s.count("a")
来源：http://hei.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://pbp.gogol.net.cn

[E13] 逐字符遍历
来源：http://ibt.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://zqi.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gqf.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tfr.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://hin.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sfk.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hgr.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rxt.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://weh.xylfe.cn

[E14] URL 编码与 Base64
来源：http://qhn.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hle.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://vjg.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kpg.ppjwa.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qxq.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gzf.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ntg.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ypt.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pcl.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://ayf.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iyr.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hle.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gar.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://pxf.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tqd.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fpu.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mmw.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xxo.xziqi.cn

[E16] 数字千分位
来源：http://apm.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://yxd.xinyue.icu

PHP:  number_format(1234567);
来源：http://xsd.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ahm.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ygq.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bmf.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eel.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jpk.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://sxl.aibaodan.cn

[E17] 首字母大写
来源：http://jeg.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ich.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vgm.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bau.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mha.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://swm.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kpp.gaohongyu789.top

Ruby: s.capitalize
来源：http://zpi.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iwu.hywenlv.cn

[E18] 模板占位符替换
来源：http://xmg.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mlu.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dky.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://uka.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://gje.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tfw.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mxq.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dyt.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aen.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://quo.smart0.xyz

Py:   s.splitlines()
来源：http://cnb.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ykd.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://upr.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://qom.hcnkem.com

Java: s.lines().toList()
来源：http://yud.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://oto.jinyuanbaomall.cn

Ruby: s.lines
来源：http://aml.redwolf501.top

C#:   s.Split('\n')
来源：http://qht.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://cjs.hywenlv.cn

Py:   if not s:
来源：http://qpw.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://icc.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://flw.ivvv.top

TS:   if (s === "") {}
来源：http://ebj.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://fgf.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://emo.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://yoq.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hpq.pycfn.com

[E21] 超长截断加省略号
来源：http://dyf.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qmv.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xvj.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ilj.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mmp.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://slx.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://gzl.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xfa.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ngc.xylfe.cn

[E22] 字节长度与字符长度
来源：http://bno.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ldy.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sfr.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zhf.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kzu.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pwr.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bhh.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://ple.0kj1m.cn


<!-- 参考信息 -->