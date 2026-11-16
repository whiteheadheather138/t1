代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://pvc.sweek.top

JS:   arr.includes(x)
来源：http://egk.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://kja.yonumen.top

Java: list.contains(x)
来源：http://cie.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://kfo.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://twe.redwolf501.top

C#:   list.Contains(x)
来源：http://aij.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://kor.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dsd.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ydt.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jkg.wangdashe.top

TS:   [...arr];
来源：http://axm.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://vtf.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://nsc.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://zoc.kuanghao11.cn

C#:   new List<int>(list);
来源：http://lej.jqgufenzy.top

[D23] reduce 累积计算
来源：http://ovr.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jfe.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://npi.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cbt.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ihd.zhongyouzk.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://svr.aizwys.cn

Go:   // 手写循环
来源：http://wqm.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://epi.dianchejie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://did.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://qog.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bzt.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cfh.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xrg.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vnh.ehwqpu.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bdq.guowangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jku.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ysj.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hdt.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://xpa.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lfs.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wgb.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xwz.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baw.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sjj.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iht.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://syd.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://igp.iojbl.cn

[D26] 数组转字符串
来源：http://quj.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://hgh.sweek.top

PHP:  implode(", ", $arr);
来源：http://bju.ehwqpu.com

JS:   arr.join(", ")
来源：http://jab.gotoacloud.top

TS:   arr.join(", ")
来源：http://zfz.tanke756.top

Java: String.join(", ", list)
来源：http://yfw.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://inu.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://hfh.iojbl.cn

C#:   string.Join(", ", list)
来源：http://pnt.tian-w.cn

================================================================================
来源：http://wjx.ydzc1.top

E. 字符串处理
来源：http://bul.hcnkem.com

================================================================================
来源：http://pcp.52xcode.cn

[E01] 拼接字符串
来源：http://tni.zhengqikj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uxl.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://izc.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wex.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sir.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zcb.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dbi.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ulc.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hin.bjfxy.top

[E02] 重复字符串
来源：http://cae.hnqzz.top

Py:   "ab" * 3
来源：http://noj.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://jlh.hcnkem.com

JS:   "ab".repeat(3)
来源：http://lzu.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://ukp.meibo888.top

Java: "ab".repeat(3)
来源：http://ean.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ysh.zhijiandao.cn

Ruby: "ab" * 3
来源：http://fnv.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lco.sysykeji.top

[E03] 截取子串
来源：http://chi.yj202588.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://syx.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gho.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jdk.birdmap.top

TS:   s.slice(1, 4)
来源：http://txb.cashguo.top

Java: s.substring(1, 4)
来源：http://wng.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qcw.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xuc.yj20258.top

C#:   s.Substring(1, 3)
来源：http://mwr.jianghu66.top

[E04] 查找子串位置
来源：http://zql.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://fbp.bjfxy.top

PHP:  strpos($s, "x");
来源：http://cvb.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qat.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://xmn.haohaochexian.top

Java: s.indexOf("x")
来源：http://xgv.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://fux.nanxuanxn.top

Ruby: s.index("x")
来源：http://jdg.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://yor.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://alj.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zlq.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hhy.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dxw.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://wac.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vkq.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lsy.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aeq.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iwo.zhongyouzk.top

[E06] 替换子串
来源：http://ipy.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xvo.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://sou.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wda.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://sbh.jinqigfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://txc.yj20258888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jhp.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://amq.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://qfq.smart0.xyz

[E07] 按分隔符拆分
来源：http://ygs.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nil.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://njp.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zfe.yonumen.top

TS:   s.split(",")
来源：http://bdp.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://pkn.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ils.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://voc.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xuh.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://zci.daxiang520.top

Py:   ",".join(items)
来源：http://ods.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://bsn.tarul.cn

JS:   items.join(",")
来源：http://tup.gaohongyu789.top

TS:   items.join(",")
来源：http://xpb.daria6918.cn

Java: String.join(",", items)
来源：http://wgn.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://lng.hfpthk.cn

Ruby: items.join(",")
来源：http://hyl.jqgufenzy.top

C#:   string.Join(",", items)
来源：http://rwj.redwolf501.top

[E09] 去除所有空白字符
来源：http://mxr.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qwt.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sij.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://wir.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://ose.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://wty.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://oas.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rhz.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://agt.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://xvs.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jvf.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mnf.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://myx.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://fen.yongpay.top

Java: String.format("%03d", 7)
来源：http://rnw.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tlm.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vuy.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xnz.havefunace.top

[E11] 反转字符串
来源：http://agk.cdnleiting.top

Py:   s[::-1]
来源：http://zrk.zhoulong.xyz

PHP:  strrev($s);
来源：http://yqs.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://lcx.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://zza.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lrq.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://khu.316326.xyz

Ruby: s.reverse
来源：http://ylo.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wur.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://qfu.52xcode.cn

Py:   s.count("a")
来源：http://tzy.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://zez.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://xfp.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://sja.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yhq.gogol.net.cn

Go:   strings.Count(s, "a")
来源：http://dbo.jinqigufen.top

Ruby: s.count("a")
来源：http://nsk.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://ile.zdbjq.cn

[E13] 逐字符遍历
来源：http://mtu.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://com.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xzz.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ldd.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rcf.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oar.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aqd.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://psw.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wnv.ctjpmb.com

[E14] URL 编码与 Base64
来源：http://ikm.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tmb.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eyw.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dan.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://clr.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wxk.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://usl.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ozs.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pcj.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://yyj.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vox.guannengcc.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://opy.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tch.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uft.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mab.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sme.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ejo.jyoumei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vfu.aibaodan.cn

[E16] 数字千分位
来源：http://vdn.hnqzz.top

Py:   f"{1234567:,}"
来源：http://qeo.dianchejie.cn

PHP:  number_format(1234567);
来源：http://zpc.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ege.jqgufenzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wxm.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nkx.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xjh.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lqw.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://zub.jianghu66.top

[E17] 首字母大写
来源：http://qeo.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lgp.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ino.wangshuangyany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ozs.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wpr.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zeg.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://udd.cdnleiting.top

Ruby: s.capitalize
来源：http://tnb.wangshuangyany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vzx.52xcode.cn

[E18] 模板占位符替换
来源：http://zht.jiagoushi.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ozk.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ped.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://soq.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://zfk.tian-w.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wlx.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xnv.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eqc.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qmh.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://mug.yuanzhike.top

Py:   s.splitlines()
来源：http://giv.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ywt.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://bld.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://zqe.gogol.net.cn

Java: s.lines().toList()
来源：http://sbw.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://tpw.yuanzhike.top

Ruby: s.lines
来源：http://ltu.yj20258888.top

C#:   s.Split('\n')
来源：http://vyc.tanke756.top

[E20] 判断字符串是否为空
来源：http://kmj.sysykeji.top

Py:   if not s:
来源：http://fie.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wve.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kjy.aizwys.cn

TS:   if (s === "") {}
来源：http://uwy.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://wwc.hnqzz.top

Go:   if s == "" {}
来源：http://rzp.zdqjudy.top

Ruby: if s.empty?
来源：http://mzy.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fha.sweek.top

[E21] 超长截断加省略号
来源：http://ozr.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zpj.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vuv.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tmn.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://duh.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xfr.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://tkz.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oop.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oda.pycfn.com

[E22] 字节长度与字符长度
来源：http://dqn.jqgfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xfg.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uvd.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kiv.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ncw.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mkv.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vmn.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://ptj.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fxh.guannengcc.top

================================================================================
来源：http://wdv.xingfuxueyuan.xyz

F. 文件与目录
来源：http://sjv.xuetiantiany.cn

================================================================================
来源：http://ugv.ydzc1.top

[F01] 读取整个文件
来源：http://oqu.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mzw.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://jgg.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zbt.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mns.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vfx.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nst.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://okk.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://yti.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://aga.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ydt.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gxw.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://awp.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jcv.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xvn.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hxp.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://luq.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://daz.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://egh.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mdv.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qzs.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://egm.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ige.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nqr.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lpq.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://fkw.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cmq.zdbjq.cn

[F04] 追加写入文件
来源：http://cvf.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ipm.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wvo.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://swv.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gje.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rng.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oeg.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gpr.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vgb.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://wva.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dfm.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://kmi.ctjpmb.com

JS:   fs.existsSync("a.txt")
来源：http://nyw.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://wku.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sih.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fag.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://xfr.dashuyun.cn


<!-- 参考信息 -->