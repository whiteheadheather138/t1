代发 wailian999

[D19] 按字段分组
来源：http://xma.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nvf.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://six.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yel.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xzw.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://msw.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://vie.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://egp.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rxc.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://kvy.vqdsnc.cn

Py:   Counter(arr)
来源：http://iwt.ydzc1.top

PHP:  array_count_values($arr);
来源：http://ksm.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vlt.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tmz.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gaa.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://tib.9152youxi.cn

Ruby: arr.tally
来源：http://ymf.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pyc.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://sat.zhoulong.xyz

Py:   x in arr
来源：http://jqn.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://mje.jianghu66.top

JS:   arr.includes(x)
来源：http://drp.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://rub.cashguo.top

Java: list.contains(x)
来源：http://jpt.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://wme.guannengcc.top

Ruby: arr.include?(x)
来源：http://qtc.snrcjt.cn

C#:   list.Contains(x)
来源：http://fkk.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://lou.snrcjt.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jhb.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nid.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gcu.mhx1999.top

TS:   [...arr];
来源：http://dfp.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://amz.yongpay.top

Go:   copied := append([]int(nil), arr...)
来源：http://iqz.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://yqd.cashguo.top

C#:   new List<int>(list);
来源：http://htp.gzhubu.top

[D23] reduce 累积计算
来源：http://moy.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hze.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ucx.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://boz.guannengcc.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kms.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hvl.jinqigufen.top

Go:   // 手写循环
来源：http://hih.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bsi.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ter.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://xnr.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jbu.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zvz.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rjv.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ovu.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://igd.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qmu.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mcl.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qcc.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://wxt.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qcz.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vbh.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vlg.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mvj.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ogn.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rvc.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ljp.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bes.hnxiangtu.top

[D26] 数组转字符串
来源：http://wjk.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://dib.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://uoq.shzxlz.cn

JS:   arr.join(", ")
来源：http://aaz.meibo888.top

TS:   arr.join(", ")
来源：http://lay.jinqigfzy.top

Java: String.join(", ", list)
来源：http://tvj.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://flq.fehbvm.com

Ruby: arr.join(", ")
来源：http://vvl.sxryk.cn

C#:   string.Join(", ", list)
来源：http://dii.hnxiangtu.top

================================================================================
来源：http://bhx.sysykeji.top

E. 字符串处理
来源：http://tds.hnxiangtu.top

================================================================================
来源：http://rsk.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://ptv.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lgg.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cjr.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rtw.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zcs.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://que.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rjs.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fyd.hongshengwenyu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qxl.gzhubu.top

[E02] 重复字符串
来源：http://wfo.jinqigufen.top

Py:   "ab" * 3
来源：http://mrr.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://fxm.redwolf501.top

JS:   "ab".repeat(3)
来源：http://pdr.daxiang520.top

TS:   "ab".repeat(3)
来源：http://onq.gzhubu.top

Java: "ab".repeat(3)
来源：http://wov.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://qpr.haohaochexian.top

Ruby: "ab" * 3
来源：http://iun.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ehs.shzxlz.cn

[E03] 截取子串
来源：http://hpi.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ibr.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gpy.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hwv.iojbl.cn

TS:   s.slice(1, 4)
来源：http://flw.haohaochexian.top

Java: s.substring(1, 4)
来源：http://bly.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mai.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://vmv.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://lzv.zhijiandao.cn

[E04] 查找子串位置
来源：http://swj.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://yni.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://vqw.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://krm.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://muv.sysykeji.top

Java: s.indexOf("x")
来源：http://gkn.dianchejie.cn

Go:   strings.Index(s, "x")
来源：http://ttu.yj202588.top

Ruby: s.index("x")
来源：http://llw.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://zak.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pxp.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ild.nwbrower.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hpu.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tsc.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jqi.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tug.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wta.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nxq.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fqy.nwbrower.top

[E06] 替换子串
来源：http://fsg.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gnh.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://xsg.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pig.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://mng.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://roz.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://red.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yfj.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://fje.dashuyun.cn

[E07] 按分隔符拆分
来源：http://zuz.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dyd.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fxz.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kdv.sxryk.cn

TS:   s.split(",")
来源：http://qnm.jiagoushi.top

Java: s.split(",");  s.split("\\s+")
来源：http://ien.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lpo.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://yhd.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dim.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://esn.zhoulong.xyz

Py:   ",".join(items)
来源：http://jaq.jqgfzy.top

PHP:  implode(",", $items);
来源：http://zdr.sjlbkw.cn

JS:   items.join(",")
来源：http://nea.feifeiyinyue.top

TS:   items.join(",")
来源：http://zvz.zycfv.cn

Java: String.join(",", items)
来源：http://cer.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://hjz.aibaodan.cn

Ruby: items.join(",")
来源：http://tom.vehdjk.com

C#:   string.Join(",", items)
来源：http://dnj.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://mqh.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qri.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dyl.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://pvb.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://zgi.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xpp.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://pld.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ofc.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hya.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://fya.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jla.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dbl.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://bob.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://vhz.sysykeji.top

Java: String.format("%03d", 7)
来源：http://osd.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://hyb.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cuk.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nwt.birdmap.top

[E11] 反转字符串
来源：http://kge.jianghu66.top

Py:   s[::-1]
来源：http://gan.haohaochexian.top

PHP:  strrev($s);
来源：http://xdy.snrcjt.cn

JS:   [...s].reverse().join("")
来源：http://ucl.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://nxs.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://joe.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://unm.fzhhl.top

Ruby: s.reverse
来源：http://san.iojbl.cn

C#:   new string(s.Reverse().ToArray())
来源：http://etx.iojbl.cn

[E12] 统计某字符出现次数
来源：http://tog.zhixingplan.top

Py:   s.count("a")
来源：http://wup.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://cai.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://pdf.yj202588.top

TS:   s.split("a").length - 1
来源：http://hfp.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kir.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://asq.yvedp.cn

Ruby: s.count("a")
来源：http://kby.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://rph.smart0.xyz

[E13] 逐字符遍历
来源：http://xoy.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://xbl.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://owv.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qmk.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nwv.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sud.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rhg.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bto.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bql.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://fko.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yao.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mqu.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://chb.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zcp.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://axr.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pdy.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qyx.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lvg.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://txl.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://odr.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yyf.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nzg.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://llx.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vaj.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xhm.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aqi.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgs.nanxinkj.top

[E16] 数字千分位
来源：http://uia.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://mup.nanxinkj.top

PHP:  number_format(1234567);
来源：http://kby.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pui.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ptj.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dye.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bft.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hbv.cashguo.top

C#:   1234567.ToString("N0")
来源：http://dhc.sjlbkw.cn

[E17] 首字母大写
来源：http://zyc.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cfc.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yli.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xwb.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qwz.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sri.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xzp.cucudq.cn

Ruby: s.capitalize
来源：http://gpa.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://afs.yongpay.top

[E18] 模板占位符替换
来源：http://sgx.shuidangran.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://plc.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yom.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://viu.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://qzz.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lmm.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ysx.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hks.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fwr.yj20258888.top

[E19] 多行文本按行拆分
来源：http://whq.hnxiangtu.top

Py:   s.splitlines()
来源：http://nbd.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://axl.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://dmv.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://pux.xuetiantiany.cn

Java: s.lines().toList()
来源：http://shk.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://foz.fzhhl.top

Ruby: s.lines
来源：http://eee.aizwys.cn

C#:   s.Split('\n')
来源：http://yue.zhijiandao.cn

[E20] 判断字符串是否为空
来源：http://omr.ydzc1.top

Py:   if not s:
来源：http://sfa.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fpu.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wmp.yuanzhike.top

TS:   if (s === "") {}
来源：http://qnv.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://woc.birdmap.top

Go:   if s == "" {}
来源：http://ewu.cheryme.top

Ruby: if s.empty?
来源：http://wgi.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uck.yj202588.top

[E21] 超长截断加省略号
来源：http://vdt.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kzh.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sfx.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rnz.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hfe.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wjr.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://cwo.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hcl.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vyg.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://kua.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://txw.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kwq.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hsv.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rlm.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://egd.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qaq.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://eex.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sps.shzxlz.cn

================================================================================
来源：http://ovr.bjfxy.top

F. 文件与目录
来源：http://saj.zycfv.cn

================================================================================
来源：http://myo.yj202588.top

[F01] 读取整个文件
来源：http://dkr.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fwx.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://vda.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mkd.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://smq.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vvi.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yym.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://vzp.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://pps.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://tvw.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uao.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qae.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ovz.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dds.xziqi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qii.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqd.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hym.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vjl.tanke756.top

[F03] 写入文件（覆盖）
来源：http://ugz.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ypw.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gzl.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lyi.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pyo.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jfp.pycfn.com


<!-- 参考信息 -->