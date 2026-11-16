代发 wailian999

[D19] 按字段分组
来源：http://txu.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yra.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hle.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kci.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zqz.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oqa.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://vkk.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qyp.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qhc.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://mcz.wangdashe.top

Py:   Counter(arr)
来源：http://mxv.yj20258.top

PHP:  array_count_values($arr);
来源：http://vtp.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uek.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mug.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://poh.ydzc1.top

Go:   // 手写 map[T]int
来源：http://qid.gotoacloud.top

Ruby: arr.tally
来源：http://dhh.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vap.ivvv.top

[D21] 判断是否包含某元素
来源：http://mec.shanyushiyangtech.top

Py:   x in arr
来源：http://rmz.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://djl.hongshengwenyu.top

JS:   arr.includes(x)
来源：http://aww.jianghu66.top

TS:   arr.includes(x)
来源：http://hxz.yangfankeji.com

Java: list.contains(x)
来源：http://pam.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://rgc.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://vhg.smart0.xyz

C#:   list.Contains(x)
来源：http://eaj.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://vlh.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zln.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mpy.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hdi.zhiwuduotai.top

TS:   [...arr];
来源：http://wbd.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://zhe.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lbe.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://xxt.guowangkeji.top

C#:   new List<int>(list);
来源：http://wdr.ybcxt.top

[D23] reduce 累积计算
来源：http://kom.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ikj.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ndl.xylfe.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dob.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gxo.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://mhi.mhx1999.top

Go:   // 手写循环
来源：http://znx.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uto.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xop.dashuyun.cn

[D24] 字典 / Map 基本操作
来源：http://sth.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ssp.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qrb.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xje.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://duv.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wmg.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jwu.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wat.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nvn.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://hbu.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mrm.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://elb.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xwf.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uct.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xro.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vju.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mhd.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nsn.zycfv.cn

[D26] 数组转字符串
来源：http://hoe.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://acb.pycfn.com

PHP:  implode(", ", $arr);
来源：http://snf.hammf.cn

JS:   arr.join(", ")
来源：http://vvc.andypj.xyz

TS:   arr.join(", ")
来源：http://fah.yanxiufei.cn

Java: String.join(", ", list)
来源：http://baw.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://aac.yfazqb.com

Ruby: arr.join(", ")
来源：http://svi.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://kcl.ywan-chungtsiang.top

================================================================================
来源：http://tia.shanyushiyangkeji.top

E. 字符串处理
来源：http://ape.aizwys.cn

================================================================================
来源：http://xpu.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://fjp.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ofu.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iho.jlsjyb.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mvn.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tgn.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rzc.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cdx.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kiu.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dzj.guannengcc.top

[E02] 重复字符串
来源：http://uol.hnqzz.top

Py:   "ab" * 3
来源：http://hep.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://fyl.zdqjudy.top

JS:   "ab".repeat(3)
来源：http://wta.nwbrower.top

TS:   "ab".repeat(3)
来源：http://jvd.pycfn.com

Java: "ab".repeat(3)
来源：http://hjs.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://plk.cdnleiting.top

Ruby: "ab" * 3
来源：http://mlv.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ppm.dashuyun.cn

[E03] 截取子串
来源：http://wps.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qah.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ewn.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lii.bbcook.cn

TS:   s.slice(1, 4)
来源：http://pog.uphjek.com

Java: s.substring(1, 4)
来源：http://bac.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kip.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://kjm.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://mol.fzhhl.top

[E04] 查找子串位置
来源：http://set.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://apg.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://ujk.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bzs.nwbrower.top

TS:   s.indexOf("x")
来源：http://hbi.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://uwa.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://hxo.yfazqb.com

Ruby: s.index("x")
来源：http://xym.xinyue.icu

C#:   s.IndexOf("x")
来源：http://knb.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xgg.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yoi.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://snt.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vfn.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kpg.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lkz.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sve.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://twg.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qho.tarul.cn

[E06] 替换子串
来源：http://ncq.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qju.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://bvo.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fwl.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://qxf.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dma.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://acq.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bdw.tarul.cn

C#:   s.Replace("a", "b")
来源：http://pmc.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://jcm.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ocq.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dte.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jbf.daria6918.cn

TS:   s.split(",")
来源：http://mgb.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://xsu.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yfb.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://iyj.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jwf.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://dwu.jlsjyb.cn

Py:   ",".join(items)
来源：http://iuv.tanke756.top

PHP:  implode(",", $items);
来源：http://gwj.yvedp.cn

JS:   items.join(",")
来源：http://pwd.hcnkem.com

TS:   items.join(",")
来源：http://rao.hesvh.cn

Java: String.join(",", items)
来源：http://xgf.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://xfd.jinqigufen.top

Ruby: items.join(",")
来源：http://eos.fktsv.cn

C#:   string.Join(",", items)
来源：http://nzb.hysaishi.cn

[E09] 去除所有空白字符
来源：http://rsv.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pxy.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://abf.dianchejie.cn

JS:   s.replace(/\s+/g, "")
来源：http://euj.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://pam.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://vbh.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://exh.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://mve.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tjc.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://ztt.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vjd.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://igq.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://ygj.smart0.xyz

TS:   "7".padStart(3, "0")
来源：http://fbs.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://fsu.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nuw.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xxv.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hhz.tian-w.cn

[E11] 反转字符串
来源：http://rte.fktsv.cn

Py:   s[::-1]
来源：http://yco.zhixingplan.top

PHP:  strrev($s);
来源：http://bcy.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://npz.meibo888.top

TS:   [...s].reverse().join("")
来源：http://pvf.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lwr.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://saz.yuanzhike.top

Ruby: s.reverse
来源：http://xih.meibo888.top

C#:   new string(s.Reverse().ToArray())
来源：http://ncq.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://qio.zhongyouzk.top

Py:   s.count("a")
来源：http://wjr.shanyushiyangkeji.top

PHP:  substr_count($s, "a");
来源：http://urs.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://ahp.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://kqv.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hhl.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://mii.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://rcg.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://jws.9152youxi.cn

[E13] 逐字符遍历
来源：http://vus.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://per.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://syh.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ass.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ejb.fzhhl.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sik.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ail.nwbrower.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wwb.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eew.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://ykh.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mzh.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://fpi.zhongyouzk.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yoh.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hfb.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jvb.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jvh.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gzd.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gdr.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://tim.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mze.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nlm.feifeiyinyue.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vmg.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zft.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kvx.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yhy.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ohn.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://opa.hfpthk.cn

[E16] 数字千分位
来源：http://bng.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://cwv.tian-w.cn

PHP:  number_format(1234567);
来源：http://kln.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://idt.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kxu.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sgk.zhijiandao.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jar.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pvj.tanke756.top

C#:   1234567.ToString("N0")
来源：http://zxh.tarul.cn

[E17] 首字母大写
来源：http://mjq.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rlc.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vco.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sdp.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gsn.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xqh.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kxv.tarul.cn

Ruby: s.capitalize
来源：http://ctn.hongshengwenyu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://npu.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://orz.andypj.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ybk.xingfuxueyuan.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pue.c1oappe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cnb.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://efj.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://srs.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wqm.andypj.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ucy.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://opt.sysykeji.top

[E19] 多行文本按行拆分
来源：http://var.quarkkingdee.top

Py:   s.splitlines()
来源：http://och.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kwu.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://ypd.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://dbo.quarkkingdee.top

Java: s.lines().toList()
来源：http://itu.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://fhp.zhaomingkeji.xyz

Ruby: s.lines
来源：http://lln.jqgufenzy.top

C#:   s.Split('\n')
来源：http://ekg.52xcode.cn

[E20] 判断字符串是否为空
来源：http://ubo.vqdsnc.cn

Py:   if not s:
来源：http://kbe.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fei.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qbn.chenjidiqi.icu

TS:   if (s === "") {}
来源：http://efd.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://cav.nanxinkj.top

Go:   if s == "" {}
来源：http://akn.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://ebe.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uii.haohaochexian.top

[E21] 超长截断加省略号
来源：http://qys.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qzf.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ypc.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jgi.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kzd.havefunace.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fve.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://cqx.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mwc.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vsz.tanke756.top

[E22] 字节长度与字符长度
来源：http://nwv.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uib.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jmv.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jxv.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bwp.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lit.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ehh.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://jgq.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fes.hcnkem.com

================================================================================
来源：http://qpi.jinqigfzy.top

F. 文件与目录
来源：http://arc.zhixingplan.top

================================================================================
来源：http://kmr.zhixingplan.top

[F01] 读取整个文件
来源：http://rzf.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hpv.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://btl.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sgy.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://epu.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://erh.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cwt.jianghu66.top

Ruby: File.read("a.txt")
来源：http://ajh.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://dqt.zycfv.cn

[F02] 逐行读取文件
来源：http://ohc.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jcc.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kkr.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sar.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nkp.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rqx.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gjo.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zvc.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ein.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://fbr.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sgz.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jjt.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://prz.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wqw.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lri.0kj1m.cn


<!-- 参考信息 -->