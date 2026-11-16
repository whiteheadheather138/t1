代发 wailian999

Java: new ArrayList<>(list);
来源：http://znz.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iby.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://gkl.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://lnm.tarul.cn

[D23] reduce 累积计算
来源：http://via.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rrv.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ilp.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://din.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gam.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://crd.nanxuanxn.top

Go:   // 手写循环
来源：http://acn.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zie.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iel.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://zzc.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lmu.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oqq.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ahw.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kfz.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vim.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://foh.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rsb.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vdd.yj20258.top

[D25] Set 集合去重与交并差
来源：http://nnd.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://utl.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://djq.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sky.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aum.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xsk.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xlk.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rya.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lur.tian-w.cn

[D26] 数组转字符串
来源：http://cqs.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://rhq.yonumen.top

PHP:  implode(", ", $arr);
来源：http://vtc.xylfe.cn

JS:   arr.join(", ")
来源：http://hxi.tian-w.cn

TS:   arr.join(", ")
来源：http://lbm.hammf.cn

Java: String.join(", ", list)
来源：http://drp.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://tvs.bbcook.cn

Ruby: arr.join(", ")
来源：http://xgj.yongpay.top

C#:   string.Join(", ", list)
来源：http://huk.sxryk.cn

================================================================================
来源：http://ndf.jqgufenzy.top

E. 字符串处理
来源：http://rvb.ctjpmb.com

================================================================================
来源：http://srq.haohaochexian.top

[E01] 拼接字符串
来源：http://msy.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pxo.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zng.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vld.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xfn.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tmb.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jmt.chenjidiqi.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dpy.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gbq.uphjek.com

[E02] 重复字符串
来源：http://dcy.uphjek.com

Py:   "ab" * 3
来源：http://fvr.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://cqq.hongshengwenyu.top

JS:   "ab".repeat(3)
来源：http://syx.epnwcf.com

TS:   "ab".repeat(3)
来源：http://kjo.sweek.top

Java: "ab".repeat(3)
来源：http://vfh.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://grd.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://fqy.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rde.andypj.xyz

[E03] 截取子串
来源：http://kvz.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yef.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tff.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ywp.yuxming.cn

TS:   s.slice(1, 4)
来源：http://wuj.zhixingplan.top

Java: s.substring(1, 4)
来源：http://biv.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fqv.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://nqo.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://lmw.zdbjq.cn

[E04] 查找子串位置
来源：http://qgx.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://igq.cashguo.top

PHP:  strpos($s, "x");
来源：http://lbe.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ahc.vehdjk.com

TS:   s.indexOf("x")
来源：http://cxs.hnxiangtu.top

Java: s.indexOf("x")
来源：http://dcz.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://xim.shangyingyoupin.top

Ruby: s.index("x")
来源：http://qtk.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://ovw.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://aki.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ubm.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vsm.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lgo.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fwc.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://drf.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tge.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lpj.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dkx.tian-w.cn

[E06] 替换子串
来源：http://hnd.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yqd.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://ykj.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rgt.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://omd.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nnc.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vyl.xziqi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ptr.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://dnt.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://xzb.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ylb.pycfn.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jae.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hyz.yj202588.top

TS:   s.split(",")
来源：http://hpk.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ekv.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kla.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://qks.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cet.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://hok.hcnkem.com

Py:   ",".join(items)
来源：http://ljy.yfazqb.com

PHP:  implode(",", $items);
来源：http://vka.yongpay.top

JS:   items.join(",")
来源：http://ywj.zhoulong.xyz

TS:   items.join(",")
来源：http://xzf.aizwys.cn

Java: String.join(",", items)
来源：http://pyl.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://ema.xuanzx.com

Ruby: items.join(",")
来源：http://ioj.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://qyx.epnwcf.com

[E09] 去除所有空白字符
来源：http://kfu.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jkq.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vpm.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://dxk.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://fnr.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://ubp.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://vrd.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://asz.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://auq.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://wry.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xao.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mbi.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://aim.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://quz.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://vdv.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vwa.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ein.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tul.aizwys.cn

[E11] 反转字符串
来源：http://vde.ctjpmb.com

Py:   s[::-1]
来源：http://nrm.guannengcc.top

PHP:  strrev($s);
来源：http://ike.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://oou.jinghuilouyu.cn

TS:   [...s].reverse().join("")
来源：http://wiu.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pri.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lld.tarul.cn

Ruby: s.reverse
来源：http://szv.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://qoc.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://hme.yj20258888.top

Py:   s.count("a")
来源：http://hzk.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://mfe.ivvv.top

JS:   s.split("a").length - 1
来源：http://wdp.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://pcv.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ipa.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://ghy.chenzaomai.com

Ruby: s.count("a")
来源：http://yny.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://zac.aibaodan.cn

[E13] 逐字符遍历
来源：http://mgn.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://dvv.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sap.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ryv.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rxj.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zvg.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ddr.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://drk.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nyx.yj20258.top

[E14] URL 编码与 Base64
来源：http://xnq.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fey.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dgk.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dvo.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kfi.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vuj.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rgi.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wkn.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mhc.jqgufenzy.top

[E15] HTML 转义 / 反转义
来源：http://gof.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dac.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fvm.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://epx.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hir.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dzd.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zkq.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nox.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wlm.pengpengdd.cyou

[E16] 数字千分位
来源：http://efy.xziqi.cn

Py:   f"{1234567:,}"
来源：http://tva.cashguo.top

PHP:  number_format(1234567);
来源：http://tpi.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jjd.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kec.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yrp.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rab.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nxi.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://eqy.316326.xyz

[E17] 首字母大写
来源：http://xxo.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xzn.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nhq.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gay.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gmu.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lnm.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pee.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://kdb.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hzs.hesvh.cn

[E18] 模板占位符替换
来源：http://dkp.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jfd.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uug.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zvz.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mwx.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bvz.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://emu.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vai.sufxvd.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iai.fzhhl.top

[E19] 多行文本按行拆分
来源：http://egc.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://dmc.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iyx.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://uaw.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://lnt.aibaodan.cn

Java: s.lines().toList()
来源：http://cnc.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://hgm.yuanzhike.top

Ruby: s.lines
来源：http://jgt.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://fox.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://mzq.gaohongyu789.top

Py:   if not s:
来源：http://sbw.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xvs.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zhi.tian-w.cn

TS:   if (s === "") {}
来源：http://koy.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://npd.daxiang520.top

Go:   if s == "" {}
来源：http://rau.9152youxi.cn

Ruby: if s.empty?
来源：http://dod.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cat.wangdashe.top

[E21] 超长截断加省略号
来源：http://mvq.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://urk.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gnf.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://reh.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jfp.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cun.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://cgf.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ohc.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lrd.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://epk.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bbs.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qmn.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gjt.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cja.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vvb.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://umi.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://cyk.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uaw.wangshuangyany.cn

================================================================================
来源：http://hsz.yongpay.top

F. 文件与目录
来源：http://sbx.pengpengdd.cyou

================================================================================
来源：http://mov.hfpthk.cn

[F01] 读取整个文件
来源：http://hxr.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yis.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://tde.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zld.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xor.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://czm.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eox.316326.xyz

Ruby: File.read("a.txt")
来源：http://qza.wangshuangyany.cn

C#:   File.ReadAllText("a.txt");
来源：http://ncz.yuxming.cn

[F02] 逐行读取文件
来源：http://brc.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zur.feifeiyinyue.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dvv.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uka.zdqjudy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eds.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gjl.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hes.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://orv.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ydt.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://dea.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://imj.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dze.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rxb.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://amh.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eqr.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ijx.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://hwe.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nvo.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://fkr.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oix.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vsq.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aye.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iyq.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://icd.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://trg.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iir.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qmu.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://zvy.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ywp.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://xwn.cheryme.top

JS:   fs.existsSync("a.txt")
来源：http://jvi.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://xlb.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vsa.yonumen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aui.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://pit.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://bvw.yj20258.top

[F06] 删除文件
来源：http://zic.316326.xyz

Py:   os.remove("a.txt")
来源：http://zfu.fehbvm.com

PHP:  unlink("a.txt");
来源：http://zdi.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://eyg.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://fiq.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tre.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://mbn.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://tbp.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://pdz.nwbrower.top

[F07] 创建目录（含多级）
来源：http://vje.xuanzx.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mfg.cucudq.cn


<!-- 参考信息 -->