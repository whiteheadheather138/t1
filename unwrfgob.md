代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zfl.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mpt.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ttp.gotoacloud.top

TS:   [...arr];
来源：http://rdn.meibo888.top

Java: new ArrayList<>(list);
来源：http://pea.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://fyf.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://gqn.zhongyouzk.top

C#:   new List<int>(list);
来源：http://lxk.daxiang520.top

[D23] reduce 累积计算
来源：http://doi.zhoulong.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://otn.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nlr.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tdj.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dbe.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wfw.daria6918.cn

Go:   // 手写循环
来源：http://emk.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ilz.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jhu.xylfe.cn

[D24] 字典 / Map 基本操作
来源：http://yus.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mdz.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zcx.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hlu.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://voy.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ody.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xul.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fva.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xkp.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://ozk.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nex.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xbb.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://llq.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ejo.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://osc.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://akm.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kfx.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qrb.bjfxy.top

[D26] 数组转字符串
来源：http://diz.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://xzm.ehwqpu.com

PHP:  implode(", ", $arr);
来源：http://qni.hywenlv.cn

JS:   arr.join(", ")
来源：http://roh.vehdjk.com

TS:   arr.join(", ")
来源：http://ycs.ppjwa.cn

Java: String.join(", ", list)
来源：http://ybe.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://sdy.fktsv.cn

Ruby: arr.join(", ")
来源：http://taq.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://dvo.yvedp.cn

================================================================================
来源：http://pxb.yfazqb.com

E. 字符串处理
来源：http://dhc.yangfankeji.com

================================================================================
来源：http://ovv.nwbrower.top

[E01] 拼接字符串
来源：http://qbg.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rcf.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zkd.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gug.guannengcc.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vyo.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mxj.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://shw.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://goc.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gna.smart0.xyz

[E02] 重复字符串
来源：http://hwl.jqgufenzy.top

Py:   "ab" * 3
来源：http://oyw.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://bzi.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://xwz.yueranfly.top

TS:   "ab".repeat(3)
来源：http://wsh.shzxlz.cn

Java: "ab".repeat(3)
来源：http://npe.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://uxr.tianlin.xyz

Ruby: "ab" * 3
来源：http://omf.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vgt.shanyushiyangkeji.top

[E03] 截取子串
来源：http://qpn.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bty.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ern.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dwu.fengsongda.top

TS:   s.slice(1, 4)
来源：http://lnh.hcnkem.com

Java: s.substring(1, 4)
来源：http://qje.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qjs.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://our.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://axk.fzhhl.top

[E04] 查找子串位置
来源：http://unz.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://uwg.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://bnf.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xjb.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://zxt.jinqigfzy.top

Java: s.indexOf("x")
来源：http://zig.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://shb.hysaishi.cn

Ruby: s.index("x")
来源：http://cfq.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://rde.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oag.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nbi.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wfl.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://izz.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qgu.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wwj.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cit.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vcy.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tjr.pengpengdd.cyou

[E06] 替换子串
来源：http://qhl.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://myt.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://xkt.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fvm.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://qpu.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://onx.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rzd.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lrn.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://kqg.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://vro.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lum.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sbu.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://pgk.jyoumei.cn

TS:   s.split(",")
来源：http://lth.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nhw.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yxz.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://uqs.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rvd.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://npw.shzxlz.cn

Py:   ",".join(items)
来源：http://xcg.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://oci.ivvv.top

JS:   items.join(",")
来源：http://wtm.hywenlv.cn

TS:   items.join(",")
来源：http://kio.gotoacloud.top

Java: String.join(",", items)
来源：http://bix.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://xpt.jinqigfzy.top

Ruby: items.join(",")
来源：http://vos.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://ftt.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://pqp.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://npu.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jmk.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://rwf.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://fmv.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://hmd.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kag.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://ryw.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qui.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://yew.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ruc.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zgc.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://kpz.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://ofd.nwbrower.top

Java: String.format("%03d", 7)
来源：http://fkt.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oeb.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wkm.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://viw.kuanghao11.cn

[E11] 反转字符串
来源：http://mmm.316326.xyz

Py:   s[::-1]
来源：http://euz.zhongyouzk.top

PHP:  strrev($s);
来源：http://tvc.yongpay.top

JS:   [...s].reverse().join("")
来源：http://bzy.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://uvl.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aod.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yfx.yanxiufei.cn

Ruby: s.reverse
来源：http://sfe.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://pqi.shuidangran.top

[E12] 统计某字符出现次数
来源：http://dkx.redwolf501.top

Py:   s.count("a")
来源：http://gtl.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://yki.meibo888.top

JS:   s.split("a").length - 1
来源：http://gnp.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://ylj.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tnn.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://bjm.cdnleiting.top

Ruby: s.count("a")
来源：http://qlg.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://bpp.ydjk.org.cn

[E13] 逐字符遍历
来源：http://yej.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://bbb.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hfp.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ewa.xuetiantiany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lhq.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cns.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pca.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kba.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kim.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://pye.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jnd.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eqg.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tcp.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://psd.jiagoushi.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://isy.bjfxy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rfw.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wzu.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jvw.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://saq.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rel.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wqp.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yeh.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ohi.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ite.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ztm.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://otq.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hgo.xuetiantiany.cn

[E16] 数字千分位
来源：http://zxj.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://kdv.xinyue.icu

PHP:  number_format(1234567);
来源：http://lyx.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ghx.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zvz.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yui.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cxs.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xux.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://bed.meibo888.top

[E17] 首字母大写
来源：http://zvp.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gwl.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rmw.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ghg.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vxk.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sdb.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qpg.chenlongwang.top

Ruby: s.capitalize
来源：http://ixa.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rmc.xziqi.cn

[E18] 模板占位符替换
来源：http://sxf.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sum.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://auf.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://fqj.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vbu.yongpay.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://luy.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nga.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fsz.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bbx.epnwcf.com

[E19] 多行文本按行拆分
来源：http://psq.sxryk.cn

Py:   s.splitlines()
来源：http://qua.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wqf.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://ksj.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://ryo.jyoumei.cn

Java: s.lines().toList()
来源：http://ckx.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://ywi.yangfankeji.com

Ruby: s.lines
来源：http://gwo.jlsjyb.cn

C#:   s.Split('\n')
来源：http://aer.xylfe.cn

[E20] 判断字符串是否为空
来源：http://vkl.shanyushiyangkeji.top

Py:   if not s:
来源：http://ftk.zdbjq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mko.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hak.tarul.cn

TS:   if (s === "") {}
来源：http://kvo.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://ujz.fehbvm.com

Go:   if s == "" {}
来源：http://ybu.birdmap.top

Ruby: if s.empty?
来源：http://uqt.svipenyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vox.pycfn.com

[E21] 超长截断加省略号
来源：http://bfm.ydjk.org.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://seu.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zof.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://apy.zhengqikj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kuo.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lyl.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://ref.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bbj.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dhr.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://ehm.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qcn.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fjp.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hpk.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fcc.dashuyun.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kmy.jyoumei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hpv.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://ghb.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://erl.sxryk.cn

================================================================================
来源：http://cjb.ywan-chungtsiang.top

F. 文件与目录
来源：http://tbz.ydjk.org.cn

================================================================================
来源：http://ipu.iojbl.cn

[F01] 读取整个文件
来源：http://lyn.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vvl.chenzaomai.com

PHP:  file_get_contents("a.txt");
来源：http://diq.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://inf.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wjt.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xna.zhijiandao.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gto.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://zat.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://nor.daxiang520.top

[F02] 逐行读取文件
来源：http://xbs.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fff.tianlin.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qeb.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://amp.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nth.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rqo.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mpc.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://frq.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rov.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://tyu.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wpe.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ewd.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wup.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sas.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mjf.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mna.mhx1999.top

Ruby: File.write("a.txt", "hi")
来源：http://vla.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qel.vqdsnc.cn

[F04] 追加写入文件
来源：http://jaz.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://whv.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wdy.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gkd.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wgg.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lpb.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wlr.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://toe.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jco.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://nyi.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tig.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://iaj.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://qjk.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://xwg.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gjv.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rjm.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://lzq.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://vyq.daria6918.cn

[F06] 删除文件
来源：http://grv.tarul.cn

Py:   os.remove("a.txt")
来源：http://ptj.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://fnv.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mpk.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://oye.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ofv.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://oiz.sweek.top


<!-- 参考信息 -->