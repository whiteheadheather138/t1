代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://fjw.yangfankeji.com

Ruby: arr.include?(x)
来源：http://nyh.hnxiangtu.top

C#:   list.Contains(x)
来源：http://gdn.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://bce.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fpc.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://age.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vdc.pengpengdd.cyou

TS:   [...arr];
来源：http://ydq.hammf.cn

Java: new ArrayList<>(list);
来源：http://fdm.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mrs.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://mcp.jqgfzy.top

C#:   new List<int>(list);
来源：http://yer.cashguo.top

[D23] reduce 累积计算
来源：http://vsg.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vpe.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lrp.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fpf.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rhz.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xoz.xuanzx.com

Go:   // 手写循环
来源：http://rqe.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nst.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pms.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://zrz.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lwh.daxiang520.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hhj.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://idi.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://enf.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qnz.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qpx.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://obz.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pyl.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://dms.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cfg.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nsy.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xxp.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uoi.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://skh.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mej.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vji.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oev.gogol.net.cn

[D26] 数组转字符串
来源：http://qye.uphjek.com

Py:   ", ".join(map(str, arr))
来源：http://jdm.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://wxy.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://tse.tarul.cn

TS:   arr.join(", ")
来源：http://avs.yj20258.top

Java: String.join(", ", list)
来源：http://pih.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://syf.guowangkeji.top

Ruby: arr.join(", ")
来源：http://exi.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://lwn.daria6918.cn

================================================================================
来源：http://owg.gogol.net.cn

E. 字符串处理
来源：http://rsx.dashuyun.cn

================================================================================
来源：http://tbz.yvedp.cn

[E01] 拼接字符串
来源：http://oxl.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://axj.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vcs.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wvb.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zvq.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nkb.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qsv.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://spd.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mew.wangdashe.top

[E02] 重复字符串
来源：http://nlt.tian-w.cn

Py:   "ab" * 3
来源：http://cql.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://ucs.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://ogl.yj202588.top

TS:   "ab".repeat(3)
来源：http://wzj.dashuyun.cn

Java: "ab".repeat(3)
来源：http://nni.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://mox.yuxming.cn

Ruby: "ab" * 3
来源：http://dyd.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://inf.jinqigfzy.top

[E03] 截取子串
来源：http://drc.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vjc.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iza.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lhs.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://rlc.yangfankeji.com

Java: s.substring(1, 4)
来源：http://jwq.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fft.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://mnr.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://nmn.sweek.top

[E04] 查找子串位置
来源：http://gab.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://unj.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://nct.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://irg.dashuyun.cn

TS:   s.indexOf("x")
来源：http://mqc.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://zis.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://kep.c1oappe.top

Ruby: s.index("x")
来源：http://ipw.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://msi.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ono.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vxf.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pah.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qpe.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bzt.zhaomingkeji.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xjh.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zyg.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jha.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qmc.pycfn.com

[E06] 替换子串
来源：http://gnk.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blz.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://jyp.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oef.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://ujp.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fqg.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ktw.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fvm.316326.xyz

C#:   s.Replace("a", "b")
来源：http://lyc.shzxlz.cn

[E07] 按分隔符拆分
来源：http://vui.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xxl.ctjpmb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lvf.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gma.snrcjt.cn

TS:   s.split(",")
来源：http://kkc.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://wdd.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://umh.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://phz.nanxuanxn.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yoh.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://qbt.ydzc1.top

Py:   ",".join(items)
来源：http://rlj.cucudq.cn

PHP:  implode(",", $items);
来源：http://cbr.yuanzhike.top

JS:   items.join(",")
来源：http://yrs.zycfv.cn

TS:   items.join(",")
来源：http://kgw.zhongyouzk.top

Java: String.join(",", items)
来源：http://yej.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://rau.fengsongda.top

Ruby: items.join(",")
来源：http://pnx.yonumen.top

C#:   string.Join(",", items)
来源：http://esz.tian-w.cn

[E09] 去除所有空白字符
来源：http://nva.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nux.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mzg.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://hth.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://tri.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://ncf.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://hsw.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://byx.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cmm.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://xmi.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wbv.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tzn.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://dxi.yueranfly.top

TS:   "7".padStart(3, "0")
来源：http://wsw.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://ouq.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nrr.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vrl.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ryj.birdmap.top

[E11] 反转字符串
来源：http://yst.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://bew.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://kmz.cheryme.top

JS:   [...s].reverse().join("")
来源：http://xkv.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://gds.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yux.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bid.gzhubu.top

Ruby: s.reverse
来源：http://vbt.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://ojm.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://dkd.316326.xyz

Py:   s.count("a")
来源：http://uok.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://oiw.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://ssi.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://bmh.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wwg.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://urg.chenzaomai.com

Ruby: s.count("a")
来源：http://asr.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://aet.zycfv.cn

[E13] 逐字符遍历
来源：http://nbv.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://slm.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rla.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://exf.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://trv.jinqigfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wbk.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yfk.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tni.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hjn.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://lga.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nod.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ilr.daxiang520.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qmu.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://plc.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ors.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mtc.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kof.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mxy.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://svk.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://svt.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jcu.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hfv.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://moj.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zwk.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bci.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lvn.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://klq.dianchejie.cn

[E16] 数字千分位
来源：http://qzd.aizwys.cn

Py:   f"{1234567:,}"
来源：http://fcz.nanxinkj.top

PHP:  number_format(1234567);
来源：http://bjw.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nwx.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vxl.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ljn.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://awt.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cwt.havefunace.top

C#:   1234567.ToString("N0")
来源：http://bnv.fanxiaobao.xyz

[E17] 首字母大写
来源：http://rgr.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sed.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://kbc.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://emo.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uaw.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kic.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aqx.feifeiyinyue.top

Ruby: s.capitalize
来源：http://hyl.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yyy.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://kia.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://chx.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eax.xziqi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rji.nanxinkj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://umx.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vpn.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://unr.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wco.sysykeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ucz.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://rum.gaohongyu789.top

Py:   s.splitlines()
来源：http://nbl.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tpg.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://rbi.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://gpq.fengsongda.top

Java: s.lines().toList()
来源：http://ycd.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://rjd.sysykeji.top

Ruby: s.lines
来源：http://hqw.gaohongyu789.top

C#:   s.Split('\n')
来源：http://kri.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://lus.ppjwa.cn

Py:   if not s:
来源：http://mfx.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lhn.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://add.ehwqpu.com

TS:   if (s === "") {}
来源：http://vke.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://sat.mhx1999.top

Go:   if s == "" {}
来源：http://abv.zhijiandao.cn

Ruby: if s.empty?
来源：http://ptv.yuanzhike.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fxr.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://glg.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nhe.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bnm.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qcp.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rik.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bvb.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://pot.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wib.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mpn.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://ype.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kta.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yvh.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dnq.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sva.316326.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://emc.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fxq.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://iaw.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oxp.zdqjudy.top

================================================================================
来源：http://ate.jyoumei.cn

F. 文件与目录
来源：http://zsw.haohaochexian.top

================================================================================
来源：http://fqd.zdqjudy.top

[F01] 读取整个文件
来源：http://frp.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hgx.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://gyd.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fbv.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vwj.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://rqp.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ofz.birdmap.top

Ruby: File.read("a.txt")
来源：http://ezm.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://lkl.fzhhl.top

[F02] 逐行读取文件
来源：http://qta.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rcz.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mwq.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rim.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://khw.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://moz.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lxl.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://stq.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wqz.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://mwb.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lby.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wpj.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iwl.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ksw.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dgo.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mue.yanxiufei.cn

Ruby: File.write("a.txt", "hi")
来源：http://zbn.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vwx.ehwqpu.com

[F04] 追加写入文件
来源：http://zmd.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yug.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lja.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hot.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://msm.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sxm.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hwl.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dcg.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vca.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://ymn.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xwk.sxryk.cn

PHP:  file_exists("a.txt");
来源：http://aab.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://wse.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://sxf.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hik.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tas.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://wyb.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://acv.ydjk.org.cn

[F06] 删除文件
来源：http://ksw.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://ecn.xuanzx.com

PHP:  unlink("a.txt");
来源：http://etq.ybcxt.top


<!-- 参考信息 -->