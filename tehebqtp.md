代发 wailian999

Java: new ArrayList<>(list);
来源：http://ezw.pycfn.com

Go:   copied := append([]int(nil), arr...)
来源：http://pul.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://upd.mhx1999.top

C#:   new List<int>(list);
来源：http://rno.andypj.xyz

[D23] reduce 累积计算
来源：http://rjq.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qbb.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nwc.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mtz.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pzl.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jyt.cashguo.top

Go:   // 手写循环
来源：http://mim.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fkf.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pry.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://avr.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://egh.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fgl.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eiv.pengpengdd.cyou

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tgl.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cvi.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tgw.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tdq.cqqwz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yap.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://ylz.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oyd.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://prr.yueranfly.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://emr.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gtu.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ppf.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fib.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xpa.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://odx.9152youxi.cn

[D26] 数组转字符串
来源：http://xcm.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://hrf.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://wdg.daria6918.cn

JS:   arr.join(", ")
来源：http://ksj.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://fsy.ydjk.org.cn

Java: String.join(", ", list)
来源：http://oav.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://wtz.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://bvk.hesvh.cn

C#:   string.Join(", ", list)
来源：http://yuy.svipenyu.cn

================================================================================
来源：http://cnt.gogol.net.cn

E. 字符串处理
来源：http://tfd.shanyushiyangkeji.top

================================================================================
来源：http://vwl.zhoulong.xyz

[E01] 拼接字符串
来源：http://oxk.aizwys.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mxi.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qrw.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://huu.havefunace.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zor.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pca.pengpengdd.cyou

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://geb.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pur.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jcl.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://zee.aibaodan.cn

Py:   "ab" * 3
来源：http://ivw.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://zaz.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://iek.hnqzz.top

TS:   "ab".repeat(3)
来源：http://nmb.wangdashe.top

Java: "ab".repeat(3)
来源：http://mea.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://kaz.ydzc1.top

Ruby: "ab" * 3
来源：http://nhi.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rzh.zhixingplan.top

[E03] 截取子串
来源：http://qza.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kho.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ggo.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://isb.xziqi.cn

TS:   s.slice(1, 4)
来源：http://rjz.jianghu66.top

Java: s.substring(1, 4)
来源：http://yim.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xyf.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xma.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://tqf.jinqigufen.top

[E04] 查找子串位置
来源：http://ttu.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://twy.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://aev.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fld.uphjek.com

TS:   s.indexOf("x")
来源：http://mjn.ivvv.top

Java: s.indexOf("x")
来源：http://ytl.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://hbg.feifeiyinyue.top

Ruby: s.index("x")
来源：http://tvu.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://xyr.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://blv.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wyb.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pfx.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hvz.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://rma.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftg.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wtf.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pxq.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ghl.havefunace.top

[E06] 替换子串
来源：http://uyk.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://esn.yj20258888.top

PHP:  str_replace("a", "b", $s);
来源：http://ywc.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qaa.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://yfw.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kso.jqgufenzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yfv.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://euk.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://oac.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://exl.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lwy.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iic.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rlt.birdmap.top

TS:   s.split(",")
来源：http://ljv.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://brq.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://osr.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://ijg.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ogq.sysykeji.top

[E08] 数组按分隔符合并
来源：http://uvy.jqgfzy.top

Py:   ",".join(items)
来源：http://mld.9152youxi.cn

PHP:  implode(",", $items);
来源：http://umm.jqgufenzy.top

JS:   items.join(",")
来源：http://uys.sweek.top

TS:   items.join(",")
来源：http://dnd.shuidangran.top

Java: String.join(",", items)
来源：http://ele.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://sby.smart0.xyz

Ruby: items.join(",")
来源：http://zht.hcnkem.com

C#:   string.Join(",", items)
来源：http://yce.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://pkj.havefunace.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qqx.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lby.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://kga.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://oeq.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://pxd.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ciy.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://ogi.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bhv.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://swi.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yhr.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wvw.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://zte.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://whi.hnqzz.top

Java: String.format("%03d", 7)
来源：http://kkh.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://eya.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iym.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jni.yvedp.cn

[E11] 反转字符串
来源：http://top.havefunace.top

Py:   s[::-1]
来源：http://uub.nanxinkj.top

PHP:  strrev($s);
来源：http://ydj.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://szf.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://zzr.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vkl.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ofd.nanxinkj.top

Ruby: s.reverse
来源：http://abv.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://zkh.hesvh.cn

[E12] 统计某字符出现次数
来源：http://hmz.fzhhl.top

Py:   s.count("a")
来源：http://aaj.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://aqg.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://eib.redwolf501.top

TS:   s.split("a").length - 1
来源：http://uvd.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://idu.cdnleiting.top

Go:   strings.Count(s, "a")
来源：http://ttl.316326.xyz

Ruby: s.count("a")
来源：http://ias.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://kig.nwbrower.top

[E13] 逐字符遍历
来源：http://rgr.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://iet.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dfu.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ruo.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://gah.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://itf.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ntx.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://pij.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xqs.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://idx.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://itt.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://whe.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cjx.ywan-chungtsiang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ptc.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mpy.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xtb.hongshengwenyu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rch.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://myr.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://liu.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://axv.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vts.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kkj.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aqv.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vnp.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cua.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://frr.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bnb.yuxming.cn

[E16] 数字千分位
来源：http://fpx.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://iqa.52xcode.cn

PHP:  number_format(1234567);
来源：http://llt.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://egs.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://lnc.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lgr.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pss.aibaodan.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rvz.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://mmt.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://xjt.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bhu.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jfh.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vvd.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xer.yj20258.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://erz.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ksu.haohaochexian.top

Ruby: s.capitalize
来源：http://cps.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qsc.dianchejie.cn

[E18] 模板占位符替换
来源：http://lsw.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ctc.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iwd.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zof.ehwqpu.com

TS:   tpl.replaceAll("{name}", name)
来源：http://mhn.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nwl.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wpo.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gnv.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xna.aibaodan.cn

[E19] 多行文本按行拆分
来源：http://zrv.yanxiufei.cn

Py:   s.splitlines()
来源：http://yxa.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dbe.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://yih.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://uha.yuxming.cn

Java: s.lines().toList()
来源：http://szs.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://dxc.shuidangran.top

Ruby: s.lines
来源：http://klw.yuxming.cn

C#:   s.Split('\n')
来源：http://rxd.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://bul.9152youxi.cn

Py:   if not s:
来源：http://nfa.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aev.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://njj.fktsv.cn

TS:   if (s === "") {}
来源：http://xmw.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://lkt.sweek.top

Go:   if s == "" {}
来源：http://ubj.xylfe.cn

Ruby: if s.empty?
来源：http://mgh.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nti.sxryk.cn

[E21] 超长截断加省略号
来源：http://xtf.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yaf.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tjl.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uux.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yts.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wkv.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://igr.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ixa.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uan.sxryk.cn

[E22] 字节长度与字符长度
来源：http://gzw.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://atm.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yqc.smart0.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fds.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ohd.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://whm.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cjr.shangyingyoupin.top

Ruby: s.bytesize;  s.length
来源：http://ese.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qlt.ctjpmb.com

================================================================================
来源：http://jzh.guannengcc.top

F. 文件与目录
来源：http://gop.yanxiufei.cn

================================================================================
来源：http://aga.yangfankeji.com

[F01] 读取整个文件
来源：http://dnu.yonumen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dkg.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://iwe.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mdl.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sjh.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qgh.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sko.yvedp.cn

Ruby: File.read("a.txt")
来源：http://xjw.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://csk.cqqwz.cn

[F02] 逐行读取文件
来源：http://eug.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ggo.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://biw.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zvo.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sjz.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://svx.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gdo.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hox.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ajf.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://prm.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qft.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fto.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ydc.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zqk.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fdc.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wyy.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://vrc.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bum.mhx1999.top

[F04] 追加写入文件
来源：http://brp.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tin.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dbe.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://txb.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fys.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pel.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://znr.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://biq.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ezb.fzhhl.top

[F05] 判断文件或目录是否存在
来源：http://txr.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gja.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://fuu.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://snh.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://jax.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://blf.ydzc1.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pbr.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://sxg.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://zop.havefunace.top

[F06] 删除文件
来源：http://jmz.cucudq.cn

Py:   os.remove("a.txt")
来源：http://bbp.yongpay.top

PHP:  unlink("a.txt");
来源：http://xkg.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://qks.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://gyn.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vgu.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://adv.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://kut.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://sjf.fengsongda.top

[F07] 创建目录（含多级）
来源：http://tys.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kgg.ppjwa.cn


<!-- 参考信息 -->