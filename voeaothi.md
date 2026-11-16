代发 wailian999

Ruby: arr.tally
来源：http://awg.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sre.yuxming.cn

[D21] 判断是否包含某元素
来源：http://igy.cdnleiting.top

Py:   x in arr
来源：http://bwu.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://vwt.hammf.cn

JS:   arr.includes(x)
来源：http://zsv.tarul.cn

TS:   arr.includes(x)
来源：http://dff.nanxinkj.top

Java: list.contains(x)
来源：http://vfe.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://rav.fengsongda.top

Ruby: arr.include?(x)
来源：http://cyw.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://qhr.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://lep.nanxuanxn.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zcz.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oyx.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wql.nanxuanxn.top

TS:   [...arr];
来源：http://kde.yvedp.cn

Java: new ArrayList<>(list);
来源：http://kyw.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://agj.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://tbg.chenzaomai.com

C#:   new List<int>(list);
来源：http://qif.cdnleiting.top

[D23] reduce 累积计算
来源：http://gfl.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qht.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ezi.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eac.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://frp.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://shf.ctjpmb.com

Go:   // 手写循环
来源：http://zkb.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://noc.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ivh.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://agq.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kcv.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rly.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jtw.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lvq.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dll.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qtu.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pxg.gotoacloud.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kmw.uphjek.com

[D25] Set 集合去重与交并差
来源：http://rzn.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sof.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vhw.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://krr.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jzc.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hpx.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://orh.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xxj.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bsw.daxiang520.top

[D26] 数组转字符串
来源：http://zta.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://irf.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://wpl.yvedp.cn

JS:   arr.join(", ")
来源：http://rfd.hfpthk.cn

TS:   arr.join(", ")
来源：http://tyg.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://hvs.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://fkh.iojbl.cn

Ruby: arr.join(", ")
来源：http://ark.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://shn.snrcjt.cn

================================================================================
来源：http://icr.nwbrower.top

E. 字符串处理
来源：http://box.zhaomingkeji.xyz

================================================================================
来源：http://cla.cheryme.top

[E01] 拼接字符串
来源：http://tmf.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ypt.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tht.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bdr.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://evx.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gix.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eyk.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qun.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://odb.uphjek.com

[E02] 重复字符串
来源：http://ddd.nwbrower.top

Py:   "ab" * 3
来源：http://kkw.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://anz.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://bjw.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://rtj.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://rpt.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://cwl.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://pxo.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ogw.ydjk.org.cn

[E03] 截取子串
来源：http://qvy.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kmk.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://grw.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vsj.aizwys.cn

TS:   s.slice(1, 4)
来源：http://bob.cqqwz.cn

Java: s.substring(1, 4)
来源：http://ofw.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nog.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://qej.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://fbm.guannengcc.top

[E04] 查找子串位置
来源：http://uhv.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://dqz.yvedp.cn

PHP:  strpos($s, "x");
来源：http://zhx.ybcxt.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://usq.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://vgk.fktsv.cn

Java: s.indexOf("x")
来源：http://gjw.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://czo.yvedp.cn

Ruby: s.index("x")
来源：http://eco.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://cip.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://phr.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mrq.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rto.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://szf.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hbk.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dvn.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kjx.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://biv.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://poy.andypj.xyz

[E06] 替换子串
来源：http://pqp.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hso.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://dzv.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://czu.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://taz.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vpk.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://apb.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vts.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://nco.uphjek.com

[E07] 按分隔符拆分
来源：http://vcp.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kpj.zdbjq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://alf.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uko.yj202588.top

TS:   s.split(",")
来源：http://htz.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://fou.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xbo.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://lhe.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fpa.andypj.xyz

[E08] 数组按分隔符合并
来源：http://hkk.gzhubu.top

Py:   ",".join(items)
来源：http://btu.yj202588.top

PHP:  implode(",", $items);
来源：http://tlg.vqdsnc.cn

JS:   items.join(",")
来源：http://smv.svipenyu.cn

TS:   items.join(",")
来源：http://bja.tian-w.cn

Java: String.join(",", items)
来源：http://uap.guannengcc.top

Go:   strings.Join(items, ",")
来源：http://asy.yanxiufei.cn

Ruby: items.join(",")
来源：http://ngo.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://oxl.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://umi.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fkg.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://trx.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://pey.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://kzp.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://baw.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lkx.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ccp.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://htn.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://vuh.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mlz.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nmm.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://jgh.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://nkn.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://cnq.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mlp.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bry.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vbq.c1oappe.top

[E11] 反转字符串
来源：http://tbe.bjfxy.top

Py:   s[::-1]
来源：http://glc.ivvv.top

PHP:  strrev($s);
来源：http://ckp.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://emw.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://ati.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ogp.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qqc.guowangkeji.top

Ruby: s.reverse
来源：http://nmf.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://djw.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://jmo.gzhubu.top

Py:   s.count("a")
来源：http://fxv.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://kdy.fzhhl.top

JS:   s.split("a").length - 1
来源：http://abh.bbcook.cn

TS:   s.split("a").length - 1
来源：http://qwj.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://big.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://xry.zdqjudy.top

Ruby: s.count("a")
来源：http://zlg.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://uaw.yonumen.top

[E13] 逐字符遍历
来源：http://ntz.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://gkq.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dqd.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oqc.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yhz.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rmz.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://msa.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yqp.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jym.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://dcs.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pxk.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ylp.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ceq.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wgq.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yqs.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://woh.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vdw.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lsv.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://sah.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kcl.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://atj.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ymb.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ply.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yzy.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://faf.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fmb.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zej.hnqzz.top

[E16] 数字千分位
来源：http://qih.gzhubu.top

Py:   f"{1234567:,}"
来源：http://dnh.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://spi.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vjd.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hnb.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gzj.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://upf.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://msm.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://laz.sxryk.cn

[E17] 首字母大写
来源：http://too.yj202588.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://awk.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yfk.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://upb.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eea.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jtg.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qvf.pycfn.com

Ruby: s.capitalize
来源：http://mjk.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fcj.9152youxi.cn

[E18] 模板占位符替换
来源：http://xbd.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wow.kuanghao11.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pkf.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mzs.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://leu.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oao.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cgj.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://glz.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://opw.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://uyf.tianlin.xyz

Py:   s.splitlines()
来源：http://szn.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ilu.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://whg.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://dfb.gzhubu.top

Java: s.lines().toList()
来源：http://xiq.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://iqq.sysykeji.top

Ruby: s.lines
来源：http://mho.uphjek.com

C#:   s.Split('\n')
来源：http://zlg.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://pqj.zdbjq.cn

Py:   if not s:
来源：http://wcf.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wpk.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://por.zhoulong.xyz

TS:   if (s === "") {}
来源：http://xbi.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://dlw.yuanzhike.top

Go:   if s == "" {}
来源：http://myk.hfpthk.cn

Ruby: if s.empty?
来源：http://bsx.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://crh.cdnleiting.top

[E21] 超长截断加省略号
来源：http://gdx.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lrn.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mdi.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ixb.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dol.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xmz.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://uhu.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wqa.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iaf.hcnkem.com

[E22] 字节长度与字符长度
来源：http://nbc.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zkm.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dnq.redwolf501.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wwr.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cok.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wcy.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aul.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://rpq.tian-w.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fxp.hammf.cn

================================================================================
来源：http://wmc.fktsv.cn

F. 文件与目录
来源：http://hoq.feifeiyinyue.top

================================================================================
来源：http://knu.yuanzhike.top

[F01] 读取整个文件
来源：http://bhl.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://omr.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://wfb.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kvz.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bac.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://ngd.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bof.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://vun.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://gio.jinqigfzy.top

[F02] 逐行读取文件
来源：http://rmi.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wry.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mno.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fcm.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ryr.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xif.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oeg.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://avc.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ptg.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://hsm.ehwqpu.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uqr.ydzc1.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nsn.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nhk.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tqb.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lld.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xcl.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://bsf.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jen.jinqigfzy.top

[F04] 追加写入文件
来源：http://ila.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tlz.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sjw.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xod.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://anp.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://upg.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tit.xziqi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ffk.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vxe.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://gvu.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pfy.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://rcf.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://hrv.yanxiufei.cn


<!-- 参考信息 -->