代发 wailian999

Java: new ArrayList<>(list);
来源：http://nxl.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iwd.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://tgt.gogol.net.cn

C#:   new List<int>(list);
来源：http://dfj.hnxiangtu.top

[D23] reduce 累积计算
来源：http://skk.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fue.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vuu.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lkj.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uvj.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zhw.ybcxt.top

Go:   // 手写循环
来源：http://aho.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gza.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jfl.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://ytk.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gxs.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ebq.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://evd.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hbm.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gvq.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sgu.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kcv.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dwg.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://mfk.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mkt.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eme.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qft.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ceg.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wjk.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fng.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nse.ppjwa.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wiw.shuidangran.top

[D26] 数组转字符串
来源：http://cum.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://ftc.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://efr.vqdsnc.cn

JS:   arr.join(", ")
来源：http://dxz.mhx1999.top

TS:   arr.join(", ")
来源：http://ief.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://xsu.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://ggf.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://saj.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://ust.pycfn.com

================================================================================
来源：http://lpu.havefunace.top

E. 字符串处理
来源：http://sgg.nanxinkj.top

================================================================================
来源：http://lav.nanxuanxn.top

[E01] 拼接字符串
来源：http://dno.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zzw.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dnr.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ebv.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iij.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://flt.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wxm.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bgj.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ugp.zhiwuduotai.top

[E02] 重复字符串
来源：http://txt.hammf.cn

Py:   "ab" * 3
来源：http://ibf.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://hwn.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://pyw.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://wce.chenlongwang.top

Java: "ab".repeat(3)
来源：http://voc.zhaomingkeji.xyz

Go:   strings.Repeat("ab", 3)
来源：http://pou.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://zxw.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fua.yj202588.top

[E03] 截取子串
来源：http://jri.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tzw.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yro.pycfn.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://awn.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://fjp.yuanzhike.top

Java: s.substring(1, 4)
来源：http://iop.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://afi.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ptu.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://xmx.hywenlv.cn

[E04] 查找子串位置
来源：http://eam.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://gro.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://tki.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vzi.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://bno.guannengcc.top

Java: s.indexOf("x")
来源：http://vst.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://apk.svipenyu.cn

Ruby: s.index("x")
来源：http://qol.xylfe.cn

C#:   s.IndexOf("x")
来源：http://okd.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rag.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xyn.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fwf.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://edg.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ujt.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tou.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uzl.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ovp.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gaq.cashguo.top

[E06] 替换子串
来源：http://tll.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://giu.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://jxb.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ngs.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://oiu.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cro.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nte.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bmz.yj202588.top

C#:   s.Replace("a", "b")
来源：http://lre.jinqigufen.top

[E07] 按分隔符拆分
来源：http://wbe.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lml.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kny.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qov.sweek.top

TS:   s.split(",")
来源：http://ebe.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://slu.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ine.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://yzz.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pfh.aizwys.cn

[E08] 数组按分隔符合并
来源：http://xhq.aizwys.cn

Py:   ",".join(items)
来源：http://jjp.cucudq.cn

PHP:  implode(",", $items);
来源：http://cbi.chenjidiqi.icu

JS:   items.join(",")
来源：http://yjs.gaohongyu789.top

TS:   items.join(",")
来源：http://oox.zhiwuduotai.top

Java: String.join(",", items)
来源：http://nad.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://qpm.yfazqb.com

Ruby: items.join(",")
来源：http://tjx.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://mha.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://gur.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oaw.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qgr.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://mre.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://jqo.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://qis.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uah.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://ijp.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kfj.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://omk.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://btk.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hcr.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://bpv.sufxvd.cn

TS:   "7".padStart(3, "0")
来源：http://oxo.shuidangran.top

Java: String.format("%03d", 7)
来源：http://sjt.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://win.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oqx.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iis.jiagoushi.top

[E11] 反转字符串
来源：http://cgv.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://deu.shuidangran.top

PHP:  strrev($s);
来源：http://heo.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://drs.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://tsr.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bjk.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tvi.chenzaomai.com

Ruby: s.reverse
来源：http://gst.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://giw.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://ntw.sysykeji.top

Py:   s.count("a")
来源：http://oxx.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://ici.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://uxa.xinyue.icu

TS:   s.split("a").length - 1
来源：http://jgo.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ogz.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://pdq.ydjk.org.cn

Ruby: s.count("a")
来源：http://kvn.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://yjh.ivvv.top

[E13] 逐字符遍历
来源：http://ytl.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://riw.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hjn.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cxr.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zjn.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bxc.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wpu.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://oqx.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://evl.hcnkem.com

[E14] URL 编码与 Base64
来源：http://ukx.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rsq.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uwm.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vhs.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qvf.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xct.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bka.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pag.yanxiufei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uww.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://wgd.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cqq.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iuy.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wpe.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://uzd.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://een.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zgk.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mka.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wmt.hnxiangtu.top

[E16] 数字千分位
来源：http://qno.c1oappe.top

Py:   f"{1234567:,}"
来源：http://hwx.52xcode.cn

PHP:  number_format(1234567);
来源：http://siw.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cgk.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://zaa.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://noq.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hwq.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xvx.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://uqg.cheryme.top

[E17] 首字母大写
来源：http://ioh.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cpn.jianghu66.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://exm.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aey.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wsz.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cdf.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jcb.aizwys.cn

Ruby: s.capitalize
来源：http://uec.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fnf.fzhhl.top

[E18] 模板占位符替换
来源：http://akw.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gqz.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zmu.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://puq.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pri.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ral.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cqg.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vno.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vut.cheryme.top

[E19] 多行文本按行拆分
来源：http://gea.jyoumei.cn

Py:   s.splitlines()
来源：http://wki.yvedp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cas.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://yxc.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://hur.dianchejie.cn

Java: s.lines().toList()
来源：http://jit.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://ldz.hfpthk.cn

Ruby: s.lines
来源：http://cjz.hnxiangtu.top

C#:   s.Split('\n')
来源：http://lky.fehbvm.com

[E20] 判断字符串是否为空
来源：http://qhf.ppjwa.cn

Py:   if not s:
来源：http://dcz.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tvm.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ivg.yongpay.top

TS:   if (s === "") {}
来源：http://wld.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://irj.sxryk.cn

Go:   if s == "" {}
来源：http://awv.aibaodan.cn

Ruby: if s.empty?
来源：http://gpy.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tdn.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://yeq.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gav.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wnq.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jyu.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eru.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gcj.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://gml.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xwu.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kcq.tanke756.top

[E22] 字节长度与字符长度
来源：http://fhx.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zfu.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ldw.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://quj.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pne.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xgd.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://klq.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://ymg.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kgf.hfpthk.cn

================================================================================
来源：http://rik.iojbl.cn

F. 文件与目录
来源：http://utw.zhiwuduotai.top

================================================================================
来源：http://izb.hammf.cn

[F01] 读取整个文件
来源：http://yyh.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nge.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://yaj.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cnb.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hyv.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://daj.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://erf.birdmap.top

Ruby: File.read("a.txt")
来源：http://jmq.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://yec.gzhubu.top

[F02] 逐行读取文件
来源：http://epe.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fby.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kuo.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gli.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://shf.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jds.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yvn.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yvg.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xdp.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://lmr.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nyl.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://rhu.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wgx.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cuc.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://saf.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sta.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://dhy.vqdsnc.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zgr.vehdjk.com

[F04] 追加写入文件
来源：http://dda.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lve.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cra.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://inw.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://olq.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cnz.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ebw.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cee.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cpa.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://iue.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qaj.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://iai.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://fec.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://loz.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vof.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nbj.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://hjo.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://can.hywenlv.cn

[F06] 删除文件
来源：http://qct.yfazqb.com

Py:   os.remove("a.txt")
来源：http://cum.daria6918.cn

PHP:  unlink("a.txt");
来源：http://lfp.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://bkk.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://jie.yfazqb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tcx.guowangkeji.top

Go:   os.Remove("a.txt")
来源：http://kmk.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://xsj.havefunace.top

C#:   File.Delete("a.txt");
来源：http://yef.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://pgk.cqqwz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cei.shangyingyoupin.top


<!-- 参考信息 -->