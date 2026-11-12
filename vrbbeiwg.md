代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://atm.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uok.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qwn.haohaochexian.top

TS:   [...arr];
来源：http://gxb.yongpay.top

Java: new ArrayList<>(list);
来源：http://qxo.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mxe.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://zdn.vqdsnc.cn

C#:   new List<int>(list);
来源：http://ccm.zhengqikj.top

[D23] reduce 累积计算
来源：http://nvr.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kll.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dcf.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cqo.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tdn.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ami.tanke756.top

Go:   // 手写循环
来源：http://sko.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://neo.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://klq.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://xzf.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bfm.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tff.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xlv.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://igs.yongpay.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fql.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tcp.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dyq.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kxk.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://lzo.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wcb.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://psg.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mfq.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mzo.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aim.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fig.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://prh.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lff.yongpay.top

[D26] 数组转字符串
来源：http://uuh.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://qbr.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://ybd.tanke756.top

JS:   arr.join(", ")
来源：http://xtu.snrcjt.cn

TS:   arr.join(", ")
来源：http://ywy.hcnkem.com

Java: String.join(", ", list)
来源：http://dnf.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://jkc.chenzaomai.com

Ruby: arr.join(", ")
来源：http://otz.tian-w.cn

C#:   string.Join(", ", list)
来源：http://znh.chenlongwang.top

================================================================================
来源：http://bis.xziqi.cn

E. 字符串处理
来源：http://xjk.yangfankeji.com

================================================================================
来源：http://pfp.aizwys.cn

[E01] 拼接字符串
来源：http://zof.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gdo.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gcy.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://flt.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vdu.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pql.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cix.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pwy.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gzr.xylfe.cn

[E02] 重复字符串
来源：http://rdo.bjfxy.top

Py:   "ab" * 3
来源：http://uzk.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://tvp.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://rwv.yj20258888.top

TS:   "ab".repeat(3)
来源：http://vds.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://ygk.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://uzu.c1oappe.top

Ruby: "ab" * 3
来源：http://dkf.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://unc.fzhhl.top

[E03] 截取子串
来源：http://hsx.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ywk.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jxz.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jgc.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://eqy.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://xin.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ien.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://emf.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://ftx.bjfxy.top

[E04] 查找子串位置
来源：http://gvl.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://alz.hesvh.cn

PHP:  strpos($s, "x");
来源：http://vyu.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zrs.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://lru.guannengcc.top

Java: s.indexOf("x")
来源：http://isj.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://ktv.nwbrower.top

Ruby: s.index("x")
来源：http://xfd.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://ecm.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://abk.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cvh.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uea.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jcp.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pdo.jyoumei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ttf.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tlq.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jya.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vew.hywenlv.cn

[E06] 替换子串
来源：http://dvg.guannengcc.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://soi.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://mps.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uzw.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://wro.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://edc.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dbr.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vgx.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://loz.redwolf501.top

[E07] 按分隔符拆分
来源：http://twr.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tll.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xkv.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hzh.cqqwz.cn

TS:   s.split(",")
来源：http://oho.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://yyo.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gpt.uphjek.com

Ruby: s.split(",");  s.split
来源：http://iqp.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bfk.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://pky.yangfankeji.com

Py:   ",".join(items)
来源：http://yld.cheryme.top

PHP:  implode(",", $items);
来源：http://pcl.bbcook.cn

JS:   items.join(",")
来源：http://bsj.tianlin.xyz

TS:   items.join(",")
来源：http://vhj.mhx1999.top

Java: String.join(",", items)
来源：http://trd.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://ykw.cqqwz.cn

Ruby: items.join(",")
来源：http://rum.zhixingplan.top

C#:   string.Join(",", items)
来源：http://bof.jianghu66.top

[E09] 去除所有空白字符
来源：http://gxb.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://llv.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wpv.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://cjy.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://otv.havefunace.top

Java: s.replaceAll("\\s+", "")
来源：http://orx.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://wvx.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://efu.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rtr.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://yuz.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cef.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ynd.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://vck.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://jlo.fengsongda.top

Java: String.format("%03d", 7)
来源：http://ian.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qfn.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lbd.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://njj.uphjek.com

[E11] 反转字符串
来源：http://yzj.jinqigufen.top

Py:   s[::-1]
来源：http://sog.snrcjt.cn

PHP:  strrev($s);
来源：http://phj.havefunace.top

JS:   [...s].reverse().join("")
来源：http://mnk.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://apz.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fae.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mbe.yfazqb.com

Ruby: s.reverse
来源：http://yfx.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ytr.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://gls.haohaochexian.top

Py:   s.count("a")
来源：http://nqd.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://gsq.fengsongda.top

JS:   s.split("a").length - 1
来源：http://gmf.sweek.top

TS:   s.split("a").length - 1
来源：http://ngt.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://taa.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://axn.52xcode.cn

Ruby: s.count("a")
来源：http://bda.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://nyt.hesvh.cn

[E13] 逐字符遍历
来源：http://fmz.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://rjj.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lfe.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fbi.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://evk.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fca.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uwi.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://kra.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ztr.wangdashe.top

[E14] URL 编码与 Base64
来源：http://vha.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nru.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ehs.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pds.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://koq.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://phb.meibo888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pjd.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iij.jqgufenzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kfk.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://qkn.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ofi.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dhd.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wda.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://aco.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://skm.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wuf.0kj1m.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fxm.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hlf.fengsongda.top

[E16] 数字千分位
来源：http://edl.pycfn.com

Py:   f"{1234567:,}"
来源：http://xpj.yueranfly.top

PHP:  number_format(1234567);
来源：http://fpx.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bsn.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vpc.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fib.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yox.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zar.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://gkg.xinyue.icu

[E17] 首字母大写
来源：http://reu.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ntv.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://qmh.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ytz.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pli.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kor.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://twf.xylfe.cn

Ruby: s.capitalize
来源：http://wdc.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zor.yanxiufei.cn

[E18] 模板占位符替换
来源：http://ccs.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lvb.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nvp.sweek.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nsi.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://arp.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qqc.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://akm.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qjk.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mgl.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://baa.hesvh.cn

Py:   s.splitlines()
来源：http://qgd.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ldf.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://mif.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://azy.jqgufenzy.top

Java: s.lines().toList()
来源：http://xgp.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://xha.fengsongda.top

Ruby: s.lines
来源：http://pfc.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://rgs.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://jdg.quarkkingdee.top

Py:   if not s:
来源：http://nfq.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://irf.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://emw.quarkkingdee.top

TS:   if (s === "") {}
来源：http://noz.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://cjo.yongpay.top

Go:   if s == "" {}
来源：http://wwk.xuanzx.com

Ruby: if s.empty?
来源：http://tic.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://exx.cashguo.top

[E21] 超长截断加省略号
来源：http://xxy.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nff.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nuv.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ubd.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eix.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wyd.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://ndo.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lju.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blm.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://yal.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://leb.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xxx.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wpw.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nzs.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://owg.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://air.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://mft.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lfy.gogol.net.cn

================================================================================
来源：http://eqp.haohaochexian.top

F. 文件与目录
来源：http://wfh.zycfv.cn

================================================================================
来源：http://wke.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://exx.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lnb.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://xfg.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kqg.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://udc.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xwu.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mir.sysykeji.top

Ruby: File.read("a.txt")
来源：http://qvn.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://thw.jiagoushi.top

[F02] 逐行读取文件
来源：http://uzu.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eva.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yve.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bia.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rij.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wbx.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://msn.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://abb.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fjq.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://ytd.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cdd.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://eih.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xwn.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wcj.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://utv.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://edi.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://czo.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jwa.feifeiyinyue.top

[F04] 追加写入文件
来源：http://wso.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ckp.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cwy.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mdt.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gkw.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://elr.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ddt.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jot.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ziw.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://txg.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zil.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://idm.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://jze.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://odg.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qri.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://val.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://wjm.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://ixx.zhaomingkeji.xyz

[F06] 删除文件
来源：http://qfl.yj20258888.top

Py:   os.remove("a.txt")
来源：http://cxi.xinyue.icu

PHP:  unlink("a.txt");
来源：http://llu.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://axw.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pav.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://goo.cheryme.top

Go:   os.Remove("a.txt")
来源：http://hmu.jinqigufen.top


<!-- 参考信息 -->