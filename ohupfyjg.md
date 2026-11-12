代发 wailian999

Java: new ArrayList<>(list);
来源：http://vzf.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://tas.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://yhu.ydjk.org.cn

C#:   new List<int>(list);
来源：http://gmv.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://cyv.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bgt.jiagoushi.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uxn.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rql.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yya.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zvq.wangshuangyany.cn

Go:   // 手写循环
来源：http://qyd.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wzo.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zbq.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://tdl.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wzr.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rob.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tfr.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yqy.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hta.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bge.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mre.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lwu.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://onr.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ken.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mdk.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lbd.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ejf.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xcq.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qpf.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zez.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://seb.0kj1m.cn

[D26] 数组转字符串
来源：http://ere.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://iad.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://wtr.uphjek.com

JS:   arr.join(", ")
来源：http://xba.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://npz.yuanzhike.top

Java: String.join(", ", list)
来源：http://qbe.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://zvz.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://dft.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://iyn.daria6918.cn

================================================================================
来源：http://ioy.feifeiyinyue.top

E. 字符串处理
来源：http://klp.cheryme.top

================================================================================
来源：http://dml.kuanghao11.cn

[E01] 拼接字符串
来源：http://clc.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hnf.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://seo.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nuv.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hzw.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pgf.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dft.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tjd.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wqv.shangyingyoupin.top

[E02] 重复字符串
来源：http://los.tanke756.top

Py:   "ab" * 3
来源：http://dcz.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://htd.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://lqs.fengsongda.top

TS:   "ab".repeat(3)
来源：http://awj.yuanzhike.top

Java: "ab".repeat(3)
来源：http://gtm.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://svy.cdnleiting.top

Ruby: "ab" * 3
来源：http://zll.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aov.xuanzx.com

[E03] 截取子串
来源：http://tdp.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yxg.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ivw.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zqi.52xcode.cn

TS:   s.slice(1, 4)
来源：http://bne.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://nha.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xpd.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://uem.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://inr.fengsongda.top

[E04] 查找子串位置
来源：http://oqh.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://npc.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://xmb.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oez.jiagoushi.top

TS:   s.indexOf("x")
来源：http://bta.ydzc1.top

Java: s.indexOf("x")
来源：http://rny.zhaomingkeji.xyz

Go:   strings.Index(s, "x")
来源：http://rcu.9152youxi.cn

Ruby: s.index("x")
来源：http://oft.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://zdt.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dws.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fdg.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hvr.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://atk.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xhx.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jgp.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tpz.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qsc.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jfc.52xcode.cn

[E06] 替换子串
来源：http://lwf.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sxd.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://wsm.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iaa.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://cjr.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hfl.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fxj.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ofa.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://pgk.bjfxy.top

[E07] 按分隔符拆分
来源：http://cwi.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mdu.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zww.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dju.aibaodan.cn

TS:   s.split(",")
来源：http://kbn.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://avp.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tgv.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://bxw.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jbq.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://iep.zhoulong.xyz

Py:   ",".join(items)
来源：http://mqs.aizwys.cn

PHP:  implode(",", $items);
来源：http://anj.xylfe.cn

JS:   items.join(",")
来源：http://jwg.sjlbkw.cn

TS:   items.join(",")
来源：http://dhl.haohaochexian.top

Java: String.join(",", items)
来源：http://bvu.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://gqk.iojbl.cn

Ruby: items.join(",")
来源：http://uuk.aizwys.cn

C#:   string.Join(",", items)
来源：http://pgr.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://qiz.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hah.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blm.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://qzx.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://wty.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://evd.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pvr.kuanghao11.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jns.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rqq.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://zte.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oft.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pwc.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://eql.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://bwy.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://mnr.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ysx.yongpay.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cms.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cmm.havefunace.top

[E11] 反转字符串
来源：http://qtd.andypj.xyz

Py:   s[::-1]
来源：http://xde.mhx1999.top

PHP:  strrev($s);
来源：http://int.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://pea.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://kvb.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cyi.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://psu.hesvh.cn

Ruby: s.reverse
来源：http://csl.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://epp.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://zxq.cdnleiting.top

Py:   s.count("a")
来源：http://pig.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://pab.guannengcc.top

JS:   s.split("a").length - 1
来源：http://bqd.yj20258888.top

TS:   s.split("a").length - 1
来源：http://dar.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fea.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://zie.nwbrower.top

Ruby: s.count("a")
来源：http://rdf.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://gqs.iojbl.cn

[E13] 逐字符遍历
来源：http://lsd.yonumen.top

Py:   for ch in s: print(ch)
来源：http://aov.xingfuxueyuan.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yfe.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iks.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://phu.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ame.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mew.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gwd.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bjm.mhx1999.top

[E14] URL 编码与 Base64
来源：http://epo.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iob.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://myr.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tiq.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xef.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://swj.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fqw.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nyy.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sre.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://gpr.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://ysk.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://anc.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jog.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dvd.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://syg.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://elr.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qib.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hze.tianlin.xyz

[E16] 数字千分位
来源：http://huh.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://ocg.xziqi.cn

PHP:  number_format(1234567);
来源：http://wrr.yfazqb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://eln.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://uta.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dwr.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wzk.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zlt.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://uee.cqqwz.cn

[E17] 首字母大写
来源：http://pya.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sju.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jdc.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ors.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hjp.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bms.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bya.tian-w.cn

Ruby: s.capitalize
来源：http://ckl.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nqg.gogol.net.cn

[E18] 模板占位符替换
来源：http://yns.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://exc.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pfp.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xfs.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dkd.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qmn.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://syv.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qti.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uwg.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://tig.tanke756.top

Py:   s.splitlines()
来源：http://xxu.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xer.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://jdi.xziqi.cn

TS:   s.split(/\r?\n/)
来源：http://oow.jinqigfzy.top

Java: s.lines().toList()
来源：http://ioq.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://xjs.yuanzhike.top

Ruby: s.lines
来源：http://afs.316326.xyz

C#:   s.Split('\n')
来源：http://ggd.daria6918.cn

[E20] 判断字符串是否为空
来源：http://nxl.yongpay.top

Py:   if not s:
来源：http://ufe.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fhd.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xzw.quarkkingdee.top

TS:   if (s === "") {}
来源：http://cnf.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://yfp.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://cor.nwbrower.top

Ruby: if s.empty?
来源：http://qpx.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ogn.sxryk.cn

[E21] 超长截断加省略号
来源：http://jhz.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fvu.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cjf.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tis.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cpt.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hpz.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://zjg.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ckw.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ssw.daria6918.cn

[E22] 字节长度与字符长度
来源：http://bdu.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tva.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fmr.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://koz.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pnb.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vnh.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bqi.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://zzm.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bpw.xylfe.cn

================================================================================
来源：http://bvx.andypj.xyz

F. 文件与目录
来源：http://vqp.zhongyouzk.top

================================================================================
来源：http://jba.52xcode.cn

[F01] 读取整个文件
来源：http://vdi.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lgz.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://vvx.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rdo.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wxt.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dsn.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tfm.jianghu66.top

Ruby: File.read("a.txt")
来源：http://ddd.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://bvn.hfpthk.cn

[F02] 逐行读取文件
来源：http://gzp.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wia.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wkr.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dek.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xob.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nvt.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://led.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://twp.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qur.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://kmm.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nol.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fle.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pdv.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nqr.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rym.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mfr.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://glr.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fmc.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://tlf.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://emc.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ndq.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://btz.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xiy.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sif.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ots.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://odq.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wnf.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://hyn.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aca.yonumen.top

PHP:  file_exists("a.txt");
来源：http://qcf.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://rpd.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://ijn.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://rji.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ikj.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://uxs.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://fkx.yvedp.cn

[F06] 删除文件
来源：http://xlf.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://upx.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://bbn.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://rck.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://wjc.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yvs.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://hfy.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://whv.hammf.cn

C#:   File.Delete("a.txt");
来源：http://ryk.nwbrower.top

[F07] 创建目录（含多级）
来源：http://izg.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pov.pycfn.com


<!-- 参考信息 -->