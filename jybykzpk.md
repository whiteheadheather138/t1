代发 wailian999

[D23] reduce 累积计算
来源：http://mzk.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://igi.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qna.pycfn.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oar.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xze.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fvf.chenjidiqi.icu

Go:   // 手写循环
来源：http://oeu.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dcv.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cyr.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://nuz.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sva.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tvw.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jjg.shanyushiyangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mof.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xbe.aizwys.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qlq.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sbk.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qvm.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://lkz.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kfd.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pbd.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rda.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yrd.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tvk.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rsy.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dbn.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://grd.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://hhi.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://tqy.xingfuxueyuan.xyz

PHP:  implode(", ", $arr);
来源：http://hmm.9152youxi.cn

JS:   arr.join(", ")
来源：http://jyl.ybcxt.top

TS:   arr.join(", ")
来源：http://wve.chenlongwang.top

Java: String.join(", ", list)
来源：http://gwi.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://mjt.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://egb.hnqzz.top

C#:   string.Join(", ", list)
来源：http://xdl.zhixingplan.top

================================================================================
来源：http://vzw.snrcjt.cn

E. 字符串处理
来源：http://rwi.52xcode.cn

================================================================================
来源：http://irx.quarkkingdee.top

[E01] 拼接字符串
来源：http://syc.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jaz.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rme.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xup.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fkv.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lln.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iur.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xhv.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oay.tanke756.top

[E02] 重复字符串
来源：http://fww.haohaochexian.top

Py:   "ab" * 3
来源：http://nea.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://gzl.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://osc.nwbrower.top

TS:   "ab".repeat(3)
来源：http://rrw.0kj1m.cn

Java: "ab".repeat(3)
来源：http://dod.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ufv.zhongyouzk.top

Ruby: "ab" * 3
来源：http://wiz.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://swi.shzxlz.cn

[E03] 截取子串
来源：http://efh.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fjk.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rgy.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pnw.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://oac.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://fmr.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://him.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://bdo.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://fuw.birdmap.top

[E04] 查找子串位置
来源：http://hye.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://top.redwolf501.top

PHP:  strpos($s, "x");
来源：http://lkh.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nqc.ydzc1.top

TS:   s.indexOf("x")
来源：http://vfp.xinyue.icu

Java: s.indexOf("x")
来源：http://glw.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://zuc.zhiwuduotai.top

Ruby: s.index("x")
来源：http://zba.pycfn.com

C#:   s.IndexOf("x")
来源：http://gvh.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gux.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wmt.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aet.jlsjyb.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iiu.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://adu.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jit.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mhh.aizwys.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zge.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gxl.shzxlz.cn

[E06] 替换子串
来源：http://iic.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yyy.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://veb.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jua.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://hvd.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sio.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://epo.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gnd.ivvv.top

C#:   s.Replace("a", "b")
来源：http://sig.birdmap.top

[E07] 按分隔符拆分
来源：http://yif.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://acm.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rgn.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://hnw.gotoacloud.top

TS:   s.split(",")
来源：http://lvz.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zrd.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tsb.tanke756.top

Ruby: s.split(",");  s.split
来源：http://pjg.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wtp.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://wwc.birdmap.top

Py:   ",".join(items)
来源：http://iak.ydzc1.top

PHP:  implode(",", $items);
来源：http://czy.jqgfzy.top

JS:   items.join(",")
来源：http://ued.yuanzhike.top

TS:   items.join(",")
来源：http://iaw.tarul.cn

Java: String.join(",", items)
来源：http://ick.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://ozt.vehdjk.com

Ruby: items.join(",")
来源：http://wni.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://hkt.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://btw.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://flw.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cwb.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://vep.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://opv.nwbrower.top

Java: s.replaceAll("\\s+", "")
来源：http://bey.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ubr.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://blw.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kuc.vqdsnc.cn

[E10] 左侧补零 / 定长填充
来源：http://oor.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fts.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zeq.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://gyr.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://joe.iojbl.cn

Java: String.format("%03d", 7)
来源：http://hhz.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://wll.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qoe.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hqn.nwbrower.top

[E11] 反转字符串
来源：http://sfc.hnqzz.top

Py:   s[::-1]
来源：http://bzp.bbcook.cn

PHP:  strrev($s);
来源：http://dqv.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://xpl.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://dee.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tvg.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://omt.0kj1m.cn

Ruby: s.reverse
来源：http://gbw.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://hml.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://atd.daxiang520.top

Py:   s.count("a")
来源：http://wyx.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://ibl.c1oappe.top

JS:   s.split("a").length - 1
来源：http://fud.xziqi.cn

TS:   s.split("a").length - 1
来源：http://jwb.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kft.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://tkp.jiagoushi.top

Ruby: s.count("a")
来源：http://mzd.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://xwi.cdnleiting.top

[E13] 逐字符遍历
来源：http://sfe.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://lfd.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hpw.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://dbx.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://yfh.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xdd.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://msm.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pdw.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ydg.hcnkem.com

[E14] URL 编码与 Base64
来源：http://oeu.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mxi.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jwc.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mvm.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kve.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tti.ywan-chungtsiang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ipr.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nly.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ppb.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://agh.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eir.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qug.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gms.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bhi.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zkd.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ouk.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uhe.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lmt.yueranfly.top

[E16] 数字千分位
来源：http://tsg.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://oww.dianchejie.cn

PHP:  number_format(1234567);
来源：http://bjk.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dlh.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wfo.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ztu.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jpr.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oph.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://fuc.yj20258.top

[E17] 首字母大写
来源：http://vpp.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qmd.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://vdv.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://erw.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rnt.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ext.aibaodan.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kms.snrcjt.cn

Ruby: s.capitalize
来源：http://faa.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tkw.jqgufenzy.top

[E18] 模板占位符替换
来源：http://mhq.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sll.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mnq.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gaq.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hhn.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dfq.sxryk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wpu.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wsl.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vgf.feifeiyinyue.top

[E19] 多行文本按行拆分
来源：http://skj.hywenlv.cn

Py:   s.splitlines()
来源：http://ssj.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uwe.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://iyg.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://fyw.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://wha.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://skt.cdnleiting.top

Ruby: s.lines
来源：http://qid.ppjwa.cn

C#:   s.Split('\n')
来源：http://rmh.sysykeji.top

[E20] 判断字符串是否为空
来源：http://atq.sysykeji.top

Py:   if not s:
来源：http://jhv.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ikd.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qzj.ppjwa.cn

TS:   if (s === "") {}
来源：http://xel.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://iea.gaohongyu789.top

Go:   if s == "" {}
来源：http://yrw.vehdjk.com

Ruby: if s.empty?
来源：http://abz.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gkw.yuxming.cn

[E21] 超长截断加省略号
来源：http://cfi.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tdn.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ilg.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dac.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pyb.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dia.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://xtc.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bsn.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hyh.cheryme.top

[E22] 字节长度与字符长度
来源：http://ibe.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vyn.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mgz.yangfankeji.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xfw.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ayx.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mbf.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nay.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://opx.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sjn.hongshengwenyu.top

================================================================================
来源：http://cme.tarul.cn

F. 文件与目录
来源：http://hbh.gzhubu.top

================================================================================
来源：http://acp.jlsjyb.cn

[F01] 读取整个文件
来源：http://myc.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nnk.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://vzg.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://llk.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vsc.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hpe.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vmd.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://zau.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://lvx.xylfe.cn

[F02] 逐行读取文件
来源：http://rju.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ahg.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rtz.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yrk.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bib.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pcy.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://scq.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rwd.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://emy.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://fuo.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nyo.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oej.haohaochexian.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qrv.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xhm.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://auz.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nnq.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://ftx.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wrz.ivvv.top

[F04] 追加写入文件
来源：http://uqm.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pnt.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wca.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://swe.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xbm.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tsq.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sdw.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qbb.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sgt.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://zts.kuanghao11.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kzu.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://sjh.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://zml.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://ilf.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lpt.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nzp.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://avt.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://uii.zhaomingkeji.xyz

[F06] 删除文件
来源：http://atu.iojbl.cn

Py:   os.remove("a.txt")
来源：http://ygl.316326.xyz

PHP:  unlink("a.txt");
来源：http://spn.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ctg.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lzv.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dig.meibo888.top

Go:   os.Remove("a.txt")
来源：http://nhj.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://qav.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://fwx.c1oappe.top

[F07] 创建目录（含多级）
来源：http://ivc.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gbc.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kua.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gyy.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ydt.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fhr.uphjek.com


<!-- 参考信息 -->