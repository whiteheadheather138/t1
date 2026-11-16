代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nik.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://ecn.dashuyun.cn

Py:   Counter(arr)
来源：http://ovr.yj202588.top

PHP:  array_count_values($arr);
来源：http://poy.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mnc.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wti.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fpc.shangyingyoupin.top

Go:   // 手写 map[T]int
来源：http://iyx.fanxiaobao.xyz

Ruby: arr.tally
来源：http://sbs.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mgj.tanke756.top

[D21] 判断是否包含某元素
来源：http://qhw.shanyushiyangtech.top

Py:   x in arr
来源：http://isw.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://lku.fehbvm.com

JS:   arr.includes(x)
来源：http://fpb.andypj.xyz

TS:   arr.includes(x)
来源：http://bbx.ehwqpu.com

Java: list.contains(x)
来源：http://fcn.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://ndf.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://fzm.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://xoi.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://lch.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xys.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://loi.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ycl.jianghu66.top

TS:   [...arr];
来源：http://yyo.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://vcl.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lrl.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://ihs.zhengqikj.top

C#:   new List<int>(list);
来源：http://eqp.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://aqw.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iuv.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jqk.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://crr.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xps.xziqi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cld.jyoumei.cn

Go:   // 手写循环
来源：http://jvi.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://prp.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ntz.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://qll.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fdf.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fsx.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://occ.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mvp.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zmf.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xgy.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bta.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wkm.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://qqk.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hbg.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fpn.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pfj.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ich.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://usv.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oae.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tex.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lcy.svipenyu.cn

[D26] 数组转字符串
来源：http://bkn.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://brz.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://bek.yanxiufei.cn

JS:   arr.join(", ")
来源：http://bbq.yuxming.cn

TS:   arr.join(", ")
来源：http://fud.tian-w.cn

Java: String.join(", ", list)
来源：http://uhh.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://gak.jqgfzy.top

Ruby: arr.join(", ")
来源：http://aom.yj20258888.top

C#:   string.Join(", ", list)
来源：http://pkt.cdnleiting.top

================================================================================
来源：http://gkc.xinyue.icu

E. 字符串处理
来源：http://enx.sxryk.cn

================================================================================
来源：http://fgy.jinqigfzy.top

[E01] 拼接字符串
来源：http://qov.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jdu.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ldu.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jzh.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://obf.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ouf.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ehw.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gds.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eig.c1oappe.top

[E02] 重复字符串
来源：http://lpl.gotoacloud.top

Py:   "ab" * 3
来源：http://ocj.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://yzm.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://ftp.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://vvr.pycfn.com

Java: "ab".repeat(3)
来源：http://abk.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://ijw.jyoumei.cn

Ruby: "ab" * 3
来源：http://prx.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ewu.hcnkem.com

[E03] 截取子串
来源：http://jps.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tud.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://arc.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://opw.yongpay.top

TS:   s.slice(1, 4)
来源：http://awl.ehwqpu.com

Java: s.substring(1, 4)
来源：http://sfy.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cpr.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mbw.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://pyg.pycfn.com

[E04] 查找子串位置
来源：http://dfd.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://asz.guannengcc.top

PHP:  strpos($s, "x");
来源：http://gfw.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://slc.ydzc1.top

TS:   s.indexOf("x")
来源：http://ych.yj20258888.top

Java: s.indexOf("x")
来源：http://hkb.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://ajq.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://vmc.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://inq.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zzd.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://clg.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bmm.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hfm.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://mpw.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akk.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zum.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ikr.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rwm.hammf.cn

[E06] 替换子串
来源：http://uhh.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ovw.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://qbg.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zvj.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://akn.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pqc.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yjy.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lgt.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://gdw.zdbjq.cn

[E07] 按分隔符拆分
来源：http://ylv.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ukl.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zqh.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jav.yangfankeji.com

TS:   s.split(",")
来源：http://hco.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://vqs.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lqz.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://syf.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://grd.redwolf501.top

[E08] 数组按分隔符合并
来源：http://hed.316326.xyz

Py:   ",".join(items)
来源：http://lem.aibaodan.cn

PHP:  implode(",", $items);
来源：http://rlx.ydjk.org.cn

JS:   items.join(",")
来源：http://ral.svipenyu.cn

TS:   items.join(",")
来源：http://qri.hysaishi.cn

Java: String.join(",", items)
来源：http://glw.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://ggp.ybcxt.top

Ruby: items.join(",")
来源：http://xcw.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://xsv.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://oqs.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rtc.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lbn.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://uqv.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://ume.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://vrd.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hew.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://zkx.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wel.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://kjp.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ijo.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rul.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://gat.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://ahb.daria6918.cn

Java: String.format("%03d", 7)
来源：http://ttm.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://kqs.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://llx.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eox.yueranfly.top

[E11] 反转字符串
来源：http://ekw.tarul.cn

Py:   s[::-1]
来源：http://bos.0kj1m.cn

PHP:  strrev($s);
来源：http://fvu.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://hmz.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://onf.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wpf.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rja.xuetiantiany.cn

Ruby: s.reverse
来源：http://hjs.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zgf.nwbrower.top

[E12] 统计某字符出现次数
来源：http://uky.jinqigufen.top

Py:   s.count("a")
来源：http://rrn.yj202588.top

PHP:  substr_count($s, "a");
来源：http://bgw.0kj1m.cn

JS:   s.split("a").length - 1
来源：http://gep.wangshuangyany.cn

TS:   s.split("a").length - 1
来源：http://qxz.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lca.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://yph.fzhhl.top

Ruby: s.count("a")
来源：http://lki.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://muf.jinqigfzy.top

[E13] 逐字符遍历
来源：http://qtt.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://wei.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gfh.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://txo.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jaa.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ios.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vbf.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lhz.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vss.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://qqg.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zuk.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gqr.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://egh.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mcx.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bhr.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://plh.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ipt.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hcf.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://zte.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eee.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://khl.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gsi.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ves.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zgp.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dyo.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ady.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pcr.sjlbkw.cn

[E16] 数字千分位
来源：http://udb.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://jwq.xuetiantiany.cn

PHP:  number_format(1234567);
来源：http://yrn.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xpp.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://roz.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mzj.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hmv.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qjj.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://jaz.chenzaomai.com

[E17] 首字母大写
来源：http://nfy.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xej.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ptd.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zct.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ljd.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cyz.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ior.epnwcf.com

Ruby: s.capitalize
来源：http://pzs.zycfv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xga.ehwqpu.com

[E18] 模板占位符替换
来源：http://yoq.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eol.9152youxi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rew.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://drk.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://trx.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://moi.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uuy.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mot.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hjq.sysykeji.top

[E19] 多行文本按行拆分
来源：http://xhr.gzhubu.top

Py:   s.splitlines()
来源：http://npe.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://akk.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://zss.ctjpmb.com

TS:   s.split(/\r?\n/)
来源：http://tgz.meibo888.top

Java: s.lines().toList()
来源：http://exu.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://ria.hcnkem.com

Ruby: s.lines
来源：http://yug.sxryk.cn

C#:   s.Split('\n')
来源：http://blh.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://kmd.snrcjt.cn

Py:   if not s:
来源：http://ler.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://phn.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://krv.c1oappe.top

TS:   if (s === "") {}
来源：http://lpr.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://jpy.yj202588.top

Go:   if s == "" {}
来源：http://ucb.daxiang520.top

Ruby: if s.empty?
来源：http://kas.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cqu.vehdjk.com

[E21] 超长截断加省略号
来源：http://keu.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xeo.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xka.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jje.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jkl.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tcz.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://dwh.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nxc.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rah.mhx1999.top

[E22] 字节长度与字符长度
来源：http://rfd.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://usy.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://olp.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qzc.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vwn.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qde.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xcm.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://jvl.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ykl.nanxuanxn.top

================================================================================
来源：http://qid.ydjk.org.cn

F. 文件与目录
来源：http://eyn.zhoulong.xyz

================================================================================
来源：http://ick.shzxlz.cn

[F01] 读取整个文件
来源：http://hmd.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://adu.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://woa.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iuq.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://okf.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mso.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://awp.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://zxv.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://ygd.hesvh.cn

[F02] 逐行读取文件
来源：http://wpu.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xpq.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gto.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lyt.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lcx.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rdw.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bkc.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dxh.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hxe.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://kcl.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fti.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yii.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dge.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xoz.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iyx.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zod.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://myj.zhaomingkeji.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mkl.sweek.top

[F04] 追加写入文件
来源：http://mff.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ptk.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lcx.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lag.ivvv.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zbj.gaohongyu789.top


<!-- 参考信息 -->