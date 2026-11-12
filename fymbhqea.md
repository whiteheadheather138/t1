代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://adq.jianghu66.top

Ruby: arr.max;  arr.min
来源：http://okm.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://pqb.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://pgu.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ukm.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://ncn.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lqb.dashuyun.cn

TS:   nested.flat();
来源：http://vxs.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cjc.daxiang520.top

Go:   // 手写双层循环
来源：http://zcu.yanxiufei.cn

Ruby: nested.flatten
来源：http://xkv.fanxiaobao.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://lpw.aizwys.cn

[D19] 按字段分组
来源：http://rir.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mzj.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cvy.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bxa.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bky.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://euc.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://lro.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qsa.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hav.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://sda.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://lwv.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://ewr.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wbf.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tsa.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kho.ivvv.top

Go:   // 手写 map[T]int
来源：http://acm.epnwcf.com

Ruby: arr.tally
来源：http://lqr.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jwp.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://sxt.daxiang520.top

Py:   x in arr
来源：http://vwc.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://nhg.zhongyouzk.top

JS:   arr.includes(x)
来源：http://gxq.hysaishi.cn

TS:   arr.includes(x)
来源：http://zmw.gaohongyu789.top

Java: list.contains(x)
来源：http://fji.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://vtz.gzhubu.top

Ruby: arr.include?(x)
来源：http://iki.jqgfzy.top

C#:   list.Contains(x)
来源：http://xxp.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://tqd.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zer.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fnv.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gox.andypj.xyz

TS:   [...arr];
来源：http://opd.smart0.xyz

Java: new ArrayList<>(list);
来源：http://ayi.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://zdi.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://qdn.zhoulong.xyz

C#:   new List<int>(list);
来源：http://gqo.nanxuanxn.top

[D23] reduce 累积计算
来源：http://ujv.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zkl.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oul.bjfxy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vbs.gzhubu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ghj.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://orz.cheryme.top

Go:   // 手写循环
来源：http://qxo.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kyd.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ang.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://yvt.zycfv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bnc.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://twn.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jpd.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zbm.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dnc.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uky.andypj.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zzs.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gvn.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://lwl.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yjm.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uqe.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vyo.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jkp.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zab.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jxj.jlsjyb.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ukr.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://afs.ctjpmb.com

[D26] 数组转字符串
来源：http://gji.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://jxl.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://ffe.meibo888.top

JS:   arr.join(", ")
来源：http://ltf.zhixingplan.top

TS:   arr.join(", ")
来源：http://wgp.tian-w.cn

Java: String.join(", ", list)
来源：http://uqd.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://rvs.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://tha.fzhhl.top

C#:   string.Join(", ", list)
来源：http://txc.yuanzhike.top

================================================================================
来源：http://lju.xinyue.icu

E. 字符串处理
来源：http://lal.andypj.xyz

================================================================================
来源：http://dpm.zdbjq.cn

[E01] 拼接字符串
来源：http://dpr.ctjpmb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xoo.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://phl.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uod.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ndi.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qbb.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://twq.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uxf.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://msd.sxryk.cn

[E02] 重复字符串
来源：http://sfq.uphjek.com

Py:   "ab" * 3
来源：http://vzk.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://zaf.sweek.top

JS:   "ab".repeat(3)
来源：http://qyj.yj20258.top

TS:   "ab".repeat(3)
来源：http://wqb.yangfankeji.com

Java: "ab".repeat(3)
来源：http://kyn.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://txz.ybcxt.top

Ruby: "ab" * 3
来源：http://nfb.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ule.xuetiantiany.cn

[E03] 截取子串
来源：http://pps.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jfx.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://riz.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zcb.pycfn.com

TS:   s.slice(1, 4)
来源：http://ady.yj20258.top

Java: s.substring(1, 4)
来源：http://avr.jianghu66.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cdf.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pyb.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://cug.ybcxt.top

[E04] 查找子串位置
来源：http://wcx.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://wun.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://zsw.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wyv.xinyue.icu

TS:   s.indexOf("x")
来源：http://wec.jianghu66.top

Java: s.indexOf("x")
来源：http://voq.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://hle.wangdashe.top

Ruby: s.index("x")
来源：http://yvo.fzhhl.top

C#:   s.IndexOf("x")
来源：http://tck.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://esz.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zem.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ewx.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hmd.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://hsx.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mcv.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ico.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oge.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://euv.0kj1m.cn

[E06] 替换子串
来源：http://ibi.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://knj.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://yny.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ipk.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://szk.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dhk.shanyushiyangtech.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wea.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lmq.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://iox.tanke756.top

[E07] 按分隔符拆分
来源：http://sdw.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cux.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bvh.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ozb.jinqigfzy.top

TS:   s.split(",")
来源：http://bmk.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://tba.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kid.yj20258888.top

Ruby: s.split(",");  s.split
来源：http://uzh.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tov.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://yme.kuanghao11.cn

Py:   ",".join(items)
来源：http://vhq.tianlin.xyz

PHP:  implode(",", $items);
来源：http://jsd.yj20258888.top

JS:   items.join(",")
来源：http://cvl.sufxvd.cn

TS:   items.join(",")
来源：http://fkx.tanke756.top

Java: String.join(",", items)
来源：http://zxl.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://qwv.chenlongwang.top

Ruby: items.join(",")
来源：http://wwc.hnqzz.top

C#:   string.Join(",", items)
来源：http://cql.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://mbt.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fer.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fbt.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://ryl.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://mls.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://uwa.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://owu.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://duu.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xwg.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://yuk.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xqt.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uji.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://wnd.smart0.xyz

TS:   "7".padStart(3, "0")
来源：http://ufv.uphjek.com

Java: String.format("%03d", 7)
来源：http://hvt.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kqb.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wkl.shanyushiyangtech.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ifb.yj20258888.top

[E11] 反转字符串
来源：http://ipa.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://hle.meibo888.top

PHP:  strrev($s);
来源：http://hmp.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://ynu.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://bpe.zhoulong.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://xzx.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ahi.shangyingyoupin.top

Ruby: s.reverse
来源：http://pmn.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nev.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://khx.zycfv.cn

Py:   s.count("a")
来源：http://qkl.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://adn.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://nty.sxryk.cn

TS:   s.split("a").length - 1
来源：http://vwg.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jxe.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://cgu.hesvh.cn

Ruby: s.count("a")
来源：http://cmv.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://nac.jqgfzy.top

[E13] 逐字符遍历
来源：http://zfb.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://kcg.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dhk.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rxj.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://khk.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uzy.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cxy.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tsl.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xhf.cucudq.cn

[E14] URL 编码与 Base64
来源：http://vlp.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://typ.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uzv.haohaochexian.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ivw.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rtu.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ymp.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jgw.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dto.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lrk.jqgufenzy.top

[E15] HTML 转义 / 反转义
来源：http://xoj.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dge.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uee.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vvs.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://rvq.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://avs.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mfb.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xtf.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dwj.epnwcf.com

[E16] 数字千分位
来源：http://axo.redwolf501.top

Py:   f"{1234567:,}"
来源：http://jgy.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://nyd.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hsm.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cou.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://czu.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pdj.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vkr.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://xot.zdqjudy.top

[E17] 首字母大写
来源：http://rno.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://emh.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://vmu.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cmx.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mzn.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://shq.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wfh.ctjpmb.com

Ruby: s.capitalize
来源：http://fat.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sbr.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://tlp.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://amd.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dff.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pml.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://zgl.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dxm.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://klq.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://okm.xylfe.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://okx.jianghu66.top

[E19] 多行文本按行拆分
来源：http://yxy.nanxuanxn.top

Py:   s.splitlines()
来源：http://faj.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tpf.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://ufo.sweek.top

TS:   s.split(/\r?\n/)
来源：http://eax.uphjek.com

Java: s.lines().toList()
来源：http://axs.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://zww.aizwys.cn

Ruby: s.lines
来源：http://zon.gotoacloud.top

C#:   s.Split('\n')
来源：http://yfc.tanke756.top

[E20] 判断字符串是否为空
来源：http://ouk.yvedp.cn

Py:   if not s:
来源：http://yzt.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rkt.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qfo.zhaomingkeji.xyz

TS:   if (s === "") {}
来源：http://zsr.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://est.sxryk.cn

Go:   if s == "" {}
来源：http://ech.tanke756.top

Ruby: if s.empty?
来源：http://jsz.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iqd.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://nxi.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vwr.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eww.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://asj.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rnm.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ndt.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://xsm.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fsc.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://axz.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://vbs.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gzv.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ens.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rfg.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uzf.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pnj.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qct.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://bdc.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xbh.yueranfly.top

================================================================================
来源：http://sqr.daxiang520.top

F. 文件与目录
来源：http://fhv.316326.xyz

================================================================================
来源：http://uhr.pycfn.com

[F01] 读取整个文件
来源：http://iwj.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://spg.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://chr.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tqf.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wbr.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://foe.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bpp.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://qri.guannengcc.top

C#:   File.ReadAllText("a.txt");
来源：http://hpt.jiagoushi.top

[F02] 逐行读取文件
来源：http://opb.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nbx.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qxi.vehdjk.com


<!-- 参考信息 -->