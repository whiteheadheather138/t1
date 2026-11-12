代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://bqb.epnwcf.com

JS:   arr.includes(x)
来源：http://vwq.yongpay.top

TS:   arr.includes(x)
来源：http://kus.uphjek.com

Java: list.contains(x)
来源：http://jfn.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://rdj.tanke756.top

Ruby: arr.include?(x)
来源：http://uxv.zdqjudy.top

C#:   list.Contains(x)
来源：http://kby.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://sph.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://feu.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lvy.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qsf.fzhhl.top

TS:   [...arr];
来源：http://qeh.yonumen.top

Java: new ArrayList<>(list);
来源：http://xpj.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gve.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://hga.tanke756.top

C#:   new List<int>(list);
来源：http://zjg.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://zid.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yff.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vnb.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aec.bjfxy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kjg.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fzv.svipenyu.cn

Go:   // 手写循环
来源：http://yoa.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vmm.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://slp.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://vct.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lyx.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://owd.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tlk.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hwp.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vsi.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zez.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mqx.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nyc.havefunace.top

[D25] Set 集合去重与交并差
来源：http://mhy.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xlq.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zew.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://akr.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://drf.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eun.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cqy.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mqu.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dqu.guannengcc.top

[D26] 数组转字符串
来源：http://tug.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://xji.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://oai.hesvh.cn

JS:   arr.join(", ")
来源：http://xpl.sysykeji.top

TS:   arr.join(", ")
来源：http://kqe.guowangkeji.top

Java: String.join(", ", list)
来源：http://lrv.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://rvz.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://mgc.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://djc.feifeiyinyue.top

================================================================================
来源：http://lha.dashuyun.cn

E. 字符串处理
来源：http://fzx.xziqi.cn

================================================================================
来源：http://vfp.vehdjk.com

[E01] 拼接字符串
来源：http://jfv.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gdp.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fgn.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eex.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bqo.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gtc.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ocv.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jtf.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://utz.cucudq.cn

[E02] 重复字符串
来源：http://lvh.nwbrower.top

Py:   "ab" * 3
来源：http://inp.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://fbz.uphjek.com

JS:   "ab".repeat(3)
来源：http://tna.yongpay.top

TS:   "ab".repeat(3)
来源：http://zyl.hesvh.cn

Java: "ab".repeat(3)
来源：http://dyp.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://nhp.zhongyouzk.top

Ruby: "ab" * 3
来源：http://pup.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nai.hesvh.cn

[E03] 截取子串
来源：http://jtp.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nup.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ujs.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qms.fzhhl.top

TS:   s.slice(1, 4)
来源：http://buq.zhengqikj.top

Java: s.substring(1, 4)
来源：http://dtk.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hox.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://oar.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://dev.jiagoushi.top

[E04] 查找子串位置
来源：http://skx.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://uwc.fehbvm.com

PHP:  strpos($s, "x");
来源：http://zfn.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wxg.tian-w.cn

TS:   s.indexOf("x")
来源：http://iew.guowangkeji.top

Java: s.indexOf("x")
来源：http://das.pycfn.com

Go:   strings.Index(s, "x")
来源：http://hsl.jianghu66.top

Ruby: s.index("x")
来源：http://drw.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://zge.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vlj.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xvi.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ole.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eqg.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sjw.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nva.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bsj.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nag.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xuw.c1oappe.top

[E06] 替换子串
来源：http://xeh.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nfv.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://mqz.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://arg.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://uzl.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fve.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uha.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qup.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://ujd.xziqi.cn

[E07] 按分隔符拆分
来源：http://fsa.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lxf.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://upy.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jue.ydjk.org.cn

TS:   s.split(",")
来源：http://wir.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://apk.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kks.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://jun.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jmc.shanyushiyangtech.top

[E08] 数组按分隔符合并
来源：http://rua.52xcode.cn

Py:   ",".join(items)
来源：http://zir.tianlin.xyz

PHP:  implode(",", $items);
来源：http://awq.bbcook.cn

JS:   items.join(",")
来源：http://rec.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://lyd.jinqigufen.top

Java: String.join(",", items)
来源：http://pgv.daxiang520.top

Go:   strings.Join(items, ",")
来源：http://cif.ydzc1.top

Ruby: items.join(",")
来源：http://pin.fzhhl.top

C#:   string.Join(",", items)
来源：http://osb.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://nee.xuanzx.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://acf.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nwr.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://pmq.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://fsj.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://wsd.yj20258888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bcg.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://sfv.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zok.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://qkk.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vht.chenzaomai.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oob.birdmap.top

JS:   "7".padStart(3, "0")
来源：http://lsa.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://jcd.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://yls.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://psv.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rsx.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ocv.epnwcf.com

[E11] 反转字符串
来源：http://mpt.hcnkem.com

Py:   s[::-1]
来源：http://mhs.yanxiufei.cn

PHP:  strrev($s);
来源：http://tub.yongpay.top

JS:   [...s].reverse().join("")
来源：http://nzb.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://wzd.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://gtd.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gxj.daxiang520.top

Ruby: s.reverse
来源：http://dix.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fvo.cheryme.top

[E12] 统计某字符出现次数
来源：http://xks.tianlin.xyz

Py:   s.count("a")
来源：http://wvh.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://lwc.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://bnx.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://coy.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qbp.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://vya.gogol.net.cn

Ruby: s.count("a")
来源：http://reb.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://syf.quarkkingdee.top

[E13] 逐字符遍历
来源：http://lbf.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://dnb.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://slw.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ukg.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://flb.hywenlv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eih.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ciw.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iiy.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sfj.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://vbx.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wqo.fzhhl.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gxv.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gcn.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zvj.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pqk.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zcg.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ort.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ndo.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://qeg.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ctr.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ydu.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://whv.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nvn.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pgc.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://thx.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lms.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xhw.jqgfzy.top

[E16] 数字千分位
来源：http://hmc.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://gdc.ydzc1.top

PHP:  number_format(1234567);
来源：http://ofs.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rch.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wer.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xse.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yie.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://odz.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://sid.smart0.xyz

[E17] 首字母大写
来源：http://ejm.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sax.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cxd.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tvw.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rsz.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ivs.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://txy.zycfv.cn

Ruby: s.capitalize
来源：http://sud.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gun.tian-w.cn

[E18] 模板占位符替换
来源：http://tqp.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tvz.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zwk.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nxd.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xit.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zok.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xxa.jinyuanbaomall.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jdr.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hqf.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://mvb.fktsv.cn

Py:   s.splitlines()
来源：http://kvz.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xup.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://hil.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://cxv.yonumen.top

Java: s.lines().toList()
来源：http://ncs.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://sos.fehbvm.com

Ruby: s.lines
来源：http://ssr.gzhubu.top

C#:   s.Split('\n')
来源：http://hic.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://cik.andypj.xyz

Py:   if not s:
来源：http://fhb.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sar.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://frh.smart0.xyz

TS:   if (s === "") {}
来源：http://dza.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://oxf.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://drd.yuanzhike.top

Ruby: if s.empty?
来源：http://orr.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aax.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://dyo.bbcook.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ecj.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uvk.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rwi.ehwqpu.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ycw.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jvh.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://gpf.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fpu.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://whp.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://bcc.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pta.meibo888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://crx.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iqn.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wpz.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tag.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kvx.zhengqikj.top

Ruby: s.bytesize;  s.length
来源：http://gqv.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dwz.pengpengdd.cyou

================================================================================
来源：http://gha.yangfankeji.com

F. 文件与目录
来源：http://cjy.shanyushiyangtech.top

================================================================================
来源：http://uku.yonumen.top

[F01] 读取整个文件
来源：http://hhf.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eds.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://bqn.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hzs.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cmn.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qrm.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xqx.yvedp.cn

Ruby: File.read("a.txt")
来源：http://zor.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://euc.gogol.net.cn

[F02] 逐行读取文件
来源：http://aam.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bvv.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qhf.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uym.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://udb.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zgd.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://omt.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gwv.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oyg.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://uuh.dianchejie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://evx.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://nhn.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://anz.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jsh.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tfk.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yfz.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://ypg.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fnf.xinyue.icu

[F04] 追加写入文件
来源：http://nrp.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mxr.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yef.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://khk.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dnj.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xut.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qra.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oly.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qjo.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://fcr.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ojv.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://nes.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://vqo.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://kgn.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vwk.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qzh.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://dcs.vqdsnc.cn


<!-- 参考信息 -->