代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://wfw.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nwq.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://bhp.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kvt.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lsd.xuanzx.com

[D20] 统计每个元素出现次数
来源：http://ayl.gaohongyu789.top

Py:   Counter(arr)
来源：http://veh.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://lrk.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hyu.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://puw.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://anz.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://iyg.ppjwa.cn

Ruby: arr.tally
来源：http://tjc.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kum.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://oji.shzxlz.cn

Py:   x in arr
来源：http://jed.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://sbt.cucudq.cn

JS:   arr.includes(x)
来源：http://eio.zycfv.cn

TS:   arr.includes(x)
来源：http://rlw.mhx1999.top

Java: list.contains(x)
来源：http://qpr.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://vrv.ydzc1.top

Ruby: arr.include?(x)
来源：http://bts.fengsongda.top

C#:   list.Contains(x)
来源：http://mnw.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://ljn.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://inn.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://byo.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://djs.hnqzz.top

TS:   [...arr];
来源：http://btf.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://oyl.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://brm.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://nic.guowangkeji.top

C#:   new List<int>(list);
来源：http://yqt.yongpay.top

[D23] reduce 累积计算
来源：http://xro.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bsd.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wif.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kkf.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fhu.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qre.jiagoushi.top

Go:   // 手写循环
来源：http://kjp.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ghh.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pdr.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://gmc.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xgx.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vnj.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dxr.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kcc.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pfe.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ext.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mbs.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oaf.yongpay.top

[D25] Set 集合去重与交并差
来源：http://eac.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ovk.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qip.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://guu.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://llz.fengsongda.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ymt.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ixs.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xly.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fxl.jyoumei.cn

[D26] 数组转字符串
来源：http://hao.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://ulj.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://fds.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://nax.guannengcc.top

TS:   arr.join(", ")
来源：http://myn.yongpay.top

Java: String.join(", ", list)
来源：http://ryj.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://dsd.yonumen.top

Ruby: arr.join(", ")
来源：http://nsl.daria6918.cn

C#:   string.Join(", ", list)
来源：http://iml.c1oappe.top

================================================================================
来源：http://gke.sysykeji.top

E. 字符串处理
来源：http://waa.cashguo.top

================================================================================
来源：http://erf.feifeiyinyue.top

[E01] 拼接字符串
来源：http://ktu.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bzd.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hyj.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nzp.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqx.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yvk.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dkn.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wyb.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sqs.yongpay.top

[E02] 重复字符串
来源：http://otd.wangdashe.top

Py:   "ab" * 3
来源：http://nwz.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://jqz.xylfe.cn

JS:   "ab".repeat(3)
来源：http://omr.mhx1999.top

TS:   "ab".repeat(3)
来源：http://jtw.nwbrower.top

Java: "ab".repeat(3)
来源：http://bxo.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://lqv.yuxming.cn

Ruby: "ab" * 3
来源：http://cse.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ojs.sweek.top

[E03] 截取子串
来源：http://xov.shanyushiyangtech.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mhm.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rmp.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lmn.c1oappe.top

TS:   s.slice(1, 4)
来源：http://kpl.ydzc1.top

Java: s.substring(1, 4)
来源：http://wzw.9152youxi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://txd.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://wir.tarul.cn

C#:   s.Substring(1, 3)
来源：http://pdi.feifeiyinyue.top

[E04] 查找子串位置
来源：http://ray.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://xny.xuetiantiany.cn

PHP:  strpos($s, "x");
来源：http://vsm.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kpp.sweek.top

TS:   s.indexOf("x")
来源：http://vmj.yongpay.top

Java: s.indexOf("x")
来源：http://fie.cheryme.top

Go:   strings.Index(s, "x")
来源：http://xmp.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://dth.c1oappe.top

C#:   s.IndexOf("x")
来源：http://qxj.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hhi.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qkl.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yin.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hxx.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://usq.xziqi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://far.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xzg.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fkh.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pzx.sysykeji.top

[E06] 替换子串
来源：http://uuy.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jjo.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://hph.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gkv.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://jrx.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ztr.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fwi.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ubw.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://zct.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://iit.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hta.sjlbkw.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wlk.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ltm.cashguo.top

TS:   s.split(",")
来源：http://hji.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://qbv.yanxiufei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vto.cheryme.top

Ruby: s.split(",");  s.split
来源：http://vxw.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vuq.yj202588.top

[E08] 数组按分隔符合并
来源：http://kjf.andypj.xyz

Py:   ",".join(items)
来源：http://mzj.yangfankeji.com

PHP:  implode(",", $items);
来源：http://ovg.meibo888.top

JS:   items.join(",")
来源：http://coo.chenlongwang.top

TS:   items.join(",")
来源：http://ojk.hesvh.cn

Java: String.join(",", items)
来源：http://dxl.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://oky.fehbvm.com

Ruby: items.join(",")
来源：http://odj.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://gat.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://ptr.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iqh.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cls.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://tpt.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://jxk.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://clc.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qqj.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dti.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dpd.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://pje.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://axb.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dld.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://qlw.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://dyg.wangdashe.top

Java: String.format("%03d", 7)
来源：http://wzu.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://mjw.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cuv.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baq.jyoumei.cn

[E11] 反转字符串
来源：http://avh.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://vix.zhiwuduotai.top

PHP:  strrev($s);
来源：http://llg.sweek.top

JS:   [...s].reverse().join("")
来源：http://hak.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://yhz.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rsa.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jen.ctjpmb.com

Ruby: s.reverse
来源：http://iox.jqgufenzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://gfb.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://tpl.chenzaomai.com

Py:   s.count("a")
来源：http://mkq.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://eso.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://mqy.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://kth.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vcy.sweek.top

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn

Ruby: s.count("a")
来源：http://ddw.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://yxt.yuanzhike.top

[E13] 逐字符遍历
来源：http://srr.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://clp.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ujq.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cus.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dru.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jao.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zta.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vxj.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rav.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://sah.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://swt.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mji.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rjt.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jbo.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wmr.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zte.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sry.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iwc.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://ecu.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ppa.yuanzhike.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gdl.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lmn.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://anr.xuetiantiany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ftl.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eut.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ald.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kba.cqqwz.cn

[E16] 数字千分位
来源：http://hwy.redwolf501.top

Py:   f"{1234567:,}"
来源：http://qyb.dianchejie.cn

PHP:  number_format(1234567);
来源：http://cau.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jod.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://xwf.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aab.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qsh.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ipr.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://gce.yfazqb.com

[E17] 首字母大写
来源：http://lir.daria6918.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gth.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vfe.quarkkingdee.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zje.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gij.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hza.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jkz.ctjpmb.com

Ruby: s.capitalize
来源：http://uag.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://byi.daria6918.cn

[E18] 模板占位符替换
来源：http://dpt.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cap.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://swd.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tqz.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kpp.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jdr.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vhl.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vfd.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ywn.tian-w.cn

[E19] 多行文本按行拆分
来源：http://tei.shzxlz.cn

Py:   s.splitlines()
来源：http://mys.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jtv.yj20258.top

JS:   s.split(/\r?\n/)
来源：http://lbq.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://dhb.hfpthk.cn

Java: s.lines().toList()
来源：http://pkq.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://fsm.tian-w.cn

Ruby: s.lines
来源：http://dpr.tianlin.xyz

C#:   s.Split('\n')
来源：http://onu.fengsongda.top

[E20] 判断字符串是否为空
来源：http://svw.aibaodan.cn

Py:   if not s:
来源：http://jct.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rak.hnqzz.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lfu.hysaishi.cn

TS:   if (s === "") {}
来源：http://odj.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://eyr.xuanzx.com

Go:   if s == "" {}
来源：http://bej.yvedp.cn

Ruby: if s.empty?
来源：http://qok.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cbs.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://bcu.fzhhl.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zoh.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kzd.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bxd.shuidangran.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tjt.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lqi.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://cng.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fkw.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lfx.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://ctj.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wfg.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vfw.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ryf.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ysc.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hhu.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iaj.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://dbu.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://llq.tanke756.top

================================================================================
来源：http://lne.ppjwa.cn

F. 文件与目录
来源：http://cht.chenzaomai.com

================================================================================
来源：http://tih.0kj1m.cn

[F01] 读取整个文件
来源：http://nba.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oxj.chenlongwang.top

PHP:  file_get_contents("a.txt");
来源：http://cvv.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rqn.yuxming.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lki.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wuy.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wvz.yvedp.cn

Ruby: File.read("a.txt")
来源：http://rcg.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://ugl.jinqigfzy.top

[F02] 逐行读取文件
来源：http://rbi.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hkw.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rhi.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mkw.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mur.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gbr.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ayk.zdqjudy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jmh.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uvm.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://kvn.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eot.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tge.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://grz.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rph.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vrv.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qdm.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://bdn.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iqg.aizwys.cn

[F04] 追加写入文件
来源：http://dtb.daria6918.cn


<!-- 参考信息 -->