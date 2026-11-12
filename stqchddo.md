代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://uzr.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://mau.smart0.xyz

TS:   arr.includes(x)
来源：http://yhm.zhoulong.xyz

Java: list.contains(x)
来源：http://fkg.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://uor.cdnleiting.top

Ruby: arr.include?(x)
来源：http://cqf.gzhubu.top

C#:   list.Contains(x)
来源：http://hfd.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://gnn.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kuy.shanyushiyangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xlq.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lcb.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://qgo.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://ree.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jgt.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://rue.tian-w.cn

C#:   new List<int>(list);
来源：http://nuc.gaohongyu789.top

[D23] reduce 累积计算
来源：http://ljq.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hrg.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uhp.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://byw.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rol.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://eup.xinyue.icu

Go:   // 手写循环
来源：http://lbg.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gym.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pgg.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://ppw.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zmy.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kal.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yme.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eoz.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tml.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fpg.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vvh.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ilh.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://lqv.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://egk.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mdk.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ljr.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gas.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fgd.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vgn.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gjh.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dlr.feifeiyinyue.top

[D26] 数组转字符串
来源：http://rcg.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://mfq.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://avs.chenlongwang.top

JS:   arr.join(", ")
来源：http://zjb.ppjwa.cn

TS:   arr.join(", ")
来源：http://vkp.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://hey.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://tfd.xinyue.icu

Ruby: arr.join(", ")
来源：http://zic.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://giy.xinyue.icu

================================================================================
来源：http://zql.jianghu66.top

E. 字符串处理
来源：http://enq.zhengqikj.top

================================================================================
来源：http://agn.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://fgn.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dus.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ssd.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bht.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wyq.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bqf.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nos.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://edi.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wtd.zhongyouzk.top

[E02] 重复字符串
来源：http://qko.epnwcf.com

Py:   "ab" * 3
来源：http://zdz.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://blh.zycfv.cn

JS:   "ab".repeat(3)
来源：http://rna.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://uwr.tanke756.top

Java: "ab".repeat(3)
来源：http://mbo.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://bsn.yangfankeji.com

Ruby: "ab" * 3
来源：http://vdv.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ttq.zdqjudy.top

[E03] 截取子串
来源：http://oaf.chenjidiqi.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uzy.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://otq.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ual.kuanghao11.cn

TS:   s.slice(1, 4)
来源：http://isv.jyoumei.cn

Java: s.substring(1, 4)
来源：http://kei.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wsc.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://pjv.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://tkx.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://itp.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://qmt.cucudq.cn

PHP:  strpos($s, "x");
来源：http://jfz.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rgi.sweek.top

TS:   s.indexOf("x")
来源：http://sac.jqgfzy.top

Java: s.indexOf("x")
来源：http://pll.cheryme.top

Go:   strings.Index(s, "x")
来源：http://irz.jinqigufen.top

Ruby: s.index("x")
来源：http://qzv.sweek.top

C#:   s.IndexOf("x")
来源：http://sqx.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tjk.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fwd.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nxb.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xcj.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kpj.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://moj.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ulg.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nes.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ikb.hnqzz.top

[E06] 替换子串
来源：http://hpi.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xqu.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://wpl.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wjt.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://bvd.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://joo.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://egv.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://keo.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://iwt.fzhhl.top

[E07] 按分隔符拆分
来源：http://mll.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ire.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eco.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://irn.guannengcc.top

TS:   s.split(",")
来源：http://aok.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://shs.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pgk.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://roj.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://soi.smart0.xyz

[E08] 数组按分隔符合并
来源：http://otb.ehwqpu.com

Py:   ",".join(items)
来源：http://agc.snrcjt.cn

PHP:  implode(",", $items);
来源：http://jxx.ehwqpu.com

JS:   items.join(",")
来源：http://ppa.aibaodan.cn

TS:   items.join(",")
来源：http://qvb.hcnkem.com

Java: String.join(",", items)
来源：http://hnx.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://akn.zhengqikj.top

Ruby: items.join(",")
来源：http://dec.daria6918.cn

C#:   string.Join(",", items)
来源：http://gde.xziqi.cn

[E09] 去除所有空白字符
来源：http://byy.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eqc.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://scr.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://bgi.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://pnh.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://lfa.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fea.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://ktb.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pkb.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://asv.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lwv.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zsd.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://uqr.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://ucc.ydzc1.top

Java: String.format("%03d", 7)
来源：http://xsl.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kqg.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lox.zhixingplan.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fsi.daxiang520.top

[E11] 反转字符串
来源：http://kjz.cucudq.cn

Py:   s[::-1]
来源：http://fmh.tarul.cn

PHP:  strrev($s);
来源：http://zdh.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://ofq.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://fms.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://sen.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://inu.yangfankeji.com

Ruby: s.reverse
来源：http://vkm.ehwqpu.com

C#:   new string(s.Reverse().ToArray())
来源：http://thl.tanke756.top

[E12] 统计某字符出现次数
来源：http://ekn.quarkkingdee.top

Py:   s.count("a")
来源：http://ijv.shanyushiyangtech.top

PHP:  substr_count($s, "a");
来源：http://glp.yueranfly.top

JS:   s.split("a").length - 1
来源：http://ddy.xziqi.cn

TS:   s.split("a").length - 1
来源：http://xuq.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ogp.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://pij.birdmap.top

Ruby: s.count("a")
来源：http://vek.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://avv.haohaochexian.top

[E13] 逐字符遍历
来源：http://dal.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://nvr.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yhx.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vao.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ijx.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cwy.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vrk.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://exv.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://grr.ivvv.top

[E14] URL 编码与 Base64
来源：http://cuw.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uhv.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zsn.nwbrower.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xkh.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mwa.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tan.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fgs.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nyz.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://paw.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://iuq.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zkt.0kj1m.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xqt.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://krb.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sru.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tvm.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ihs.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://heo.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mhg.tanke756.top

[E16] 数字千分位
来源：http://tye.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://bxb.gzhubu.top

PHP:  number_format(1234567);
来源：http://jzu.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lyi.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qvl.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eln.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wvo.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://izq.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://fpl.redwolf501.top

[E17] 首字母大写
来源：http://ylr.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ixt.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gym.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mpa.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dfj.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://itn.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qjn.yfazqb.com

Ruby: s.capitalize
来源：http://xgr.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mxq.cashguo.top

[E18] 模板占位符替换
来源：http://tzm.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ioa.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dyj.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yfm.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sum.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wts.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wdo.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vhu.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lfx.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://puw.jyoumei.cn

Py:   s.splitlines()
来源：http://sun.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bff.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://zaa.yangfankeji.com

TS:   s.split(/\r?\n/)
来源：http://zhn.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://yad.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://cts.hfpthk.cn

Ruby: s.lines
来源：http://uuw.vehdjk.com

C#:   s.Split('\n')
来源：http://suy.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://jqb.nanxinkj.top

Py:   if not s:
来源：http://wte.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://igj.zhixingplan.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hep.pycfn.com

TS:   if (s === "") {}
来源：http://yik.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://gti.zdbjq.cn

Go:   if s == "" {}
来源：http://nbi.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://rmx.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cnm.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://weo.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bay.zhiwuduotai.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fyl.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://olk.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vke.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://crv.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://ahr.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blf.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ckd.ydzc1.top

[E22] 字节长度与字符长度
来源：http://ujd.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://axt.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wby.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pdz.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wgj.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rpg.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://abs.ppjwa.cn

Ruby: s.bytesize;  s.length
来源：http://ckq.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dfk.epnwcf.com

================================================================================
来源：http://njh.birdmap.top

F. 文件与目录
来源：http://upr.sweek.top

================================================================================
来源：http://vof.shangyingyoupin.top

[F01] 读取整个文件
来源：http://nvv.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pel.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://umc.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hbh.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fkl.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rfo.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iut.hesvh.cn

Ruby: File.read("a.txt")
来源：http://yir.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://qtm.ydzc1.top

[F02] 逐行读取文件
来源：http://jzc.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uug.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bpl.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tbo.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fni.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kmb.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fqh.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zaw.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sil.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://vmn.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ipa.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ocf.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rph.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rio.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://obl.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://maj.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://cjl.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://flu.316326.xyz

[F04] 追加写入文件
来源：http://ukh.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mog.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rvr.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mzz.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xts.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hqz.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hqq.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://arq.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://upb.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://qex.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pvr.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://rhv.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://gjx.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://brq.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hdr.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cqn.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://nyp.yj20258.top


<!-- 参考信息 -->