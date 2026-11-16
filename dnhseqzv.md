代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://ism.hammf.cn

JS:   arr.includes(x)
来源：http://eqq.9152youxi.cn

TS:   arr.includes(x)
来源：http://fhs.ydzc1.top

Java: list.contains(x)
来源：http://cpi.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://ddb.yangfankeji.com

Ruby: arr.include?(x)
来源：http://cmk.zhijiandao.cn

C#:   list.Contains(x)
来源：http://vfv.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://iyq.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dfj.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://can.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uqr.kuanghao11.cn

TS:   [...arr];
来源：http://fer.yfazqb.com

Java: new ArrayList<>(list);
来源：http://iox.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://odf.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://ffa.fehbvm.com

C#:   new List<int>(list);
来源：http://pjw.fzhhl.top

[D23] reduce 累积计算
来源：http://uru.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ylq.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://njw.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wzo.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yjg.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ufx.tarul.cn

Go:   // 手写循环
来源：http://jea.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vry.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xsn.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://vrr.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mfd.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jrg.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zyh.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://brl.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tzi.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ydr.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xon.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kpt.yj202588.top

[D25] Set 集合去重与交并差
来源：http://gru.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rrr.yanxiufei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jpo.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kvy.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wrt.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ctp.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://flh.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://run.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vhb.zhongyouzk.top

[D26] 数组转字符串
来源：http://zwg.ydzc1.top

Py:   ", ".join(map(str, arr))
来源：http://asm.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://dxb.ctjpmb.com

JS:   arr.join(", ")
来源：http://xtf.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://ktp.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://dor.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://rrl.yj20258888.top

Ruby: arr.join(", ")
来源：http://gkj.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://oig.zhengqikj.top

================================================================================
来源：http://xgb.cdnleiting.top

E. 字符串处理
来源：http://hol.hammf.cn

================================================================================
来源：http://fwd.ydjk.org.cn

[E01] 拼接字符串
来源：http://ulj.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tvt.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pcm.jyoumei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yyx.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://etz.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jyy.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sak.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dxp.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://evp.iojbl.cn

[E02] 重复字符串
来源：http://ona.nwbrower.top

Py:   "ab" * 3
来源：http://wio.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://ada.ybcxt.top

JS:   "ab".repeat(3)
来源：http://doy.tian-w.cn

TS:   "ab".repeat(3)
来源：http://nct.jqgfzy.top

Java: "ab".repeat(3)
来源：http://amu.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://fkl.cucudq.cn

Ruby: "ab" * 3
来源：http://bun.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vgm.yvedp.cn

[E03] 截取子串
来源：http://hhw.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://coj.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pgw.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jnx.fzhhl.top

TS:   s.slice(1, 4)
来源：http://cxs.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://sms.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hal.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://lse.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://qwj.haohaochexian.top

[E04] 查找子串位置
来源：http://gsu.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://fyp.fehbvm.com

PHP:  strpos($s, "x");
来源：http://eop.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bsq.52xcode.cn

TS:   s.indexOf("x")
来源：http://wpo.kuanghao11.cn

Java: s.indexOf("x")
来源：http://aes.yonumen.top

Go:   strings.Index(s, "x")
来源：http://uhi.zhiwuduotai.top

Ruby: s.index("x")
来源：http://gip.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://jss.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://veu.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tvu.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qnj.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tft.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gdy.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ukq.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yhm.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gnr.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qwz.jianghu66.top

[E06] 替换子串
来源：http://hrx.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rxt.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://rrr.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dfv.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://fot.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mwc.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gvz.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wgl.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://pcy.chenzaomai.com

[E07] 按分隔符拆分
来源：http://hig.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://apb.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qpk.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://abm.shanyushiyangtech.top

TS:   s.split(",")
来源：http://okh.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://waf.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mkl.ivvv.top

Ruby: s.split(",");  s.split
来源：http://vmv.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://spw.havefunace.top

[E08] 数组按分隔符合并
来源：http://jvj.redwolf501.top

Py:   ",".join(items)
来源：http://dhi.svipenyu.cn

PHP:  implode(",", $items);
来源：http://uzs.jiagoushi.top

JS:   items.join(",")
来源：http://fvq.sysykeji.top

TS:   items.join(",")
来源：http://qiq.tanke756.top

Java: String.join(",", items)
来源：http://myi.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://qnr.zhiwuduotai.top

Ruby: items.join(",")
来源：http://twf.yuxming.cn

C#:   string.Join(",", items)
来源：http://wtl.hywenlv.cn

[E09] 去除所有空白字符
来源：http://xyn.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ifc.wangdashe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hfp.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://kgd.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://gtm.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://vcs.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yyy.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://jxh.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jtj.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://dfg.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tle.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qll.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://tgz.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://rkh.nwbrower.top

Java: String.format("%03d", 7)
来源：http://xwa.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://hmy.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mzc.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vjd.cqqwz.cn

[E11] 反转字符串
来源：http://ydv.zhixingplan.top

Py:   s[::-1]
来源：http://gch.xuanzx.com

PHP:  strrev($s);
来源：http://wre.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://tag.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://srz.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ljd.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ope.cqqwz.cn

Ruby: s.reverse
来源：http://wgs.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://xfb.iojbl.cn

[E12] 统计某字符出现次数
来源：http://iha.yuanzhike.top

Py:   s.count("a")
来源：http://cxu.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://xzl.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://cdi.fanxiaobao.xyz

TS:   s.split("a").length - 1
来源：http://xtu.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iyt.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://wvd.nanxuanxn.top

Ruby: s.count("a")
来源：http://jas.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://yhy.tanke756.top

[E13] 逐字符遍历
来源：http://brv.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://ptn.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fts.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jov.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wsf.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gua.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ign.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mml.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rzd.sxryk.cn

[E14] URL 编码与 Base64
来源：http://weo.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oic.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ojx.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zml.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zsk.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ezh.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fgg.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oug.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qhf.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://gey.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vdv.hammf.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ssr.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jze.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://big.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kpw.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kzw.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bot.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zgm.feifeiyinyue.top

[E16] 数字千分位
来源：http://wbq.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://tew.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://urs.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://bia.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tjq.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://axt.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://avw.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://myq.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://std.tanke756.top

[E17] 首字母大写
来源：http://rrc.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ihv.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jga.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rcg.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wwp.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qfd.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sgv.yj20258888.top

Ruby: s.capitalize
来源：http://cum.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ser.gaohongyu789.top

[E18] 模板占位符替换
来源：http://wta.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zae.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ayn.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hfe.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tqq.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nls.uphjek.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qpn.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tut.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xvi.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://pjh.snrcjt.cn

Py:   s.splitlines()
来源：http://wlf.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wom.xingfuxueyuan.xyz

JS:   s.split(/\r?\n/)
来源：http://iol.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://gus.yuanzhike.top

Java: s.lines().toList()
来源：http://uce.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://ohu.shangyingyoupin.top

Ruby: s.lines
来源：http://lgf.hysaishi.cn

C#:   s.Split('\n')
来源：http://gil.havefunace.top

[E20] 判断字符串是否为空
来源：http://nmi.zhaomingkeji.xyz

Py:   if not s:
来源：http://bgb.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sbk.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aqz.tanke756.top

TS:   if (s === "") {}
来源：http://dxy.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://rld.wangshuangyany.cn

Go:   if s == "" {}
来源：http://bzp.jinqigufen.top

Ruby: if s.empty?
来源：http://vmz.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yyy.iojbl.cn

[E21] 超长截断加省略号
来源：http://xsj.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://avs.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://luy.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kgt.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rhh.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pea.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://tsa.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rdm.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xis.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://jtl.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lay.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rkq.yangfankeji.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vqz.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gap.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wyp.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uwa.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://lxm.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ihl.redwolf501.top

================================================================================
来源：http://ywc.zhengqikj.top

F. 文件与目录
来源：http://eqy.cucudq.cn

================================================================================
来源：http://clt.yj202588.top

[F01] 读取整个文件
来源：http://tku.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ftw.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://wyp.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://slw.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pgw.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gjv.zhijiandao.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fla.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://mnk.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://vio.fktsv.cn

[F02] 逐行读取文件
来源：http://kjn.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ojm.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xji.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zab.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zeq.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rle.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qhz.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rqv.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yog.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://ooh.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yla.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vtm.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yzx.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://shk.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yia.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iov.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://mpe.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://feb.meibo888.top

[F04] 追加写入文件
来源：http://izk.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ukx.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bdk.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kgn.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ugb.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vfy.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aqv.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hyy.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wav.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://mgn.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tlc.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://fvl.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://tkq.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://lne.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ejk.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zdq.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://evk.9152youxi.cn


<!-- 参考信息 -->