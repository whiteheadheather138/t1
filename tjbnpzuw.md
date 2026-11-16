代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kmi.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nug.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pae.haohaochexian.top

TS:   [...arr];
来源：http://cxz.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://rsc.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://fhe.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://dbp.andypj.xyz

C#:   new List<int>(list);
来源：http://xmh.aizwys.cn

[D23] reduce 累积计算
来源：http://qaa.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ltz.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hdk.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mbz.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pgl.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mph.cqqwz.cn

Go:   // 手写循环
来源：http://fzj.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://duu.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qxu.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://zju.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xtw.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vyy.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eoz.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://axr.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://odr.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yrj.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://luw.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mae.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://oyt.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qbt.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rrt.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jmc.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yns.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cwa.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lnn.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pju.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tjh.hammf.cn

[D26] 数组转字符串
来源：http://ued.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://ajp.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://lqm.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://hdh.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://dlj.sweek.top

Java: String.join(", ", list)
来源：http://hln.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://rsg.xuanzx.com

Ruby: arr.join(", ")
来源：http://kdg.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://uix.vehdjk.com

================================================================================
来源：http://myv.ivvv.top

E. 字符串处理
来源：http://cem.yongpay.top

================================================================================
来源：http://cfc.ydzc1.top

[E01] 拼接字符串
来源：http://uit.zhengqikj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://evn.andypj.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://khe.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rkr.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lua.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ijo.yanxiufei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uec.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://exs.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ene.tian-w.cn

[E02] 重复字符串
来源：http://dku.yuxming.cn

Py:   "ab" * 3
来源：http://zbz.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://gxs.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://ymq.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://eem.hfpthk.cn

Java: "ab".repeat(3)
来源：http://ext.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://rzc.zhijiandao.cn

Ruby: "ab" * 3
来源：http://mia.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sdg.zycfv.cn

[E03] 截取子串
来源：http://vyn.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xny.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zef.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vcm.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://iao.zhixingplan.top

Java: s.substring(1, 4)
来源：http://ugv.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ktk.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://qvb.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://hsv.ctjpmb.com

[E04] 查找子串位置
来源：http://kxx.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://xcx.aizwys.cn

PHP:  strpos($s, "x");
来源：http://vdv.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lgi.hcnkem.com

TS:   s.indexOf("x")
来源：http://nrw.epnwcf.com

Java: s.indexOf("x")
来源：http://gwe.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://oul.guannengcc.top

Ruby: s.index("x")
来源：http://olo.daxiang520.top

C#:   s.IndexOf("x")
来源：http://ghm.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://mpo.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gcq.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pme.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ttj.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jss.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pen.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ptm.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yqa.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dak.gaohongyu789.top

[E06] 替换子串
来源：http://bsr.svipenyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sfy.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://kzj.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oge.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://rnt.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ktv.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aco.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pel.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://nfs.shzxlz.cn

[E07] 按分隔符拆分
来源：http://ieq.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zgj.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cvl.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qed.316326.xyz

TS:   s.split(",")
来源：http://alz.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://eiv.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ype.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://cyv.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pfk.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://jtw.zhongyouzk.top

Py:   ",".join(items)
来源：http://vsk.chenzaomai.com

PHP:  implode(",", $items);
来源：http://cms.havefunace.top

JS:   items.join(",")
来源：http://nkn.redwolf501.top

TS:   items.join(",")
来源：http://mgf.yuxming.cn

Java: String.join(",", items)
来源：http://mop.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://ntl.sysykeji.top

Ruby: items.join(",")
来源：http://jbw.shangyingyoupin.top

C#:   string.Join(",", items)
来源：http://oim.52xcode.cn

[E09] 去除所有空白字符
来源：http://ltz.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uix.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bdy.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://cgi.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://myb.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://koi.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://qez.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://duk.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nbb.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://rsl.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ffj.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hqc.ybcxt.top

JS:   "7".padStart(3, "0")
来源：http://lee.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://ehk.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://fqj.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pkq.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bon.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://spr.gogol.net.cn

[E11] 反转字符串
来源：http://pfe.zhixingplan.top

Py:   s[::-1]
来源：http://oqq.tanke756.top

PHP:  strrev($s);
来源：http://hby.316326.xyz

JS:   [...s].reverse().join("")
来源：http://hrm.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://fsy.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sus.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://tvj.c1oappe.top

Ruby: s.reverse
来源：http://ogd.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pam.wangdashe.top

[E12] 统计某字符出现次数
来源：http://hef.hywenlv.cn

Py:   s.count("a")
来源：http://mmd.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://dek.birdmap.top

JS:   s.split("a").length - 1
来源：http://swz.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://kpi.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://msd.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://cel.hongshengwenyu.top

Ruby: s.count("a")
来源：http://bmd.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://zet.zycfv.cn

[E13] 逐字符遍历
来源：http://qel.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://iaj.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://krp.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gzq.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qdg.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dql.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://osq.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cvs.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://prw.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://hzv.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vlf.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mss.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cvf.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jpe.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://phr.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hej.ywan-chungtsiang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aln.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bza.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://wmz.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qgk.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kwo.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pyu.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sxe.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kak.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://erd.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yfc.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://loj.fzhhl.top

[E16] 数字千分位
来源：http://bjb.52xcode.cn

Py:   f"{1234567:,}"
来源：http://stg.xylfe.cn

PHP:  number_format(1234567);
来源：http://ifd.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zsb.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://jxr.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://myg.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mzq.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lqs.uphjek.com

C#:   1234567.ToString("N0")
来源：http://azx.yj20258.top

[E17] 首字母大写
来源：http://gac.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yqf.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vqx.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kry.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xmx.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vnt.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vlr.zhijiandao.cn

Ruby: s.capitalize
来源：http://nlj.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vrw.andypj.xyz

[E18] 模板占位符替换
来源：http://bma.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kng.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pts.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://put.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://qyu.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://frv.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ekg.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mnw.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://moq.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://wru.hnqzz.top

Py:   s.splitlines()
来源：http://mfs.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wzy.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://htq.havefunace.top

TS:   s.split(/\r?\n/)
来源：http://aea.gogol.net.cn

Java: s.lines().toList()
来源：http://jzy.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://wjr.hfpthk.cn

Ruby: s.lines
来源：http://rqy.bjfxy.top

C#:   s.Split('\n')
来源：http://ifc.shanyushiyangkeji.top

[E20] 判断字符串是否为空
来源：http://ryu.xziqi.cn

Py:   if not s:
来源：http://pks.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mwl.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ute.hnqzz.top

TS:   if (s === "") {}
来源：http://lyg.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://jda.cashguo.top

Go:   if s == "" {}
来源：http://xtg.0kj1m.cn

Ruby: if s.empty?
来源：http://gbd.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hnt.shuidangran.top

[E21] 超长截断加省略号
来源：http://omw.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ywb.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aoo.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lwi.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qjb.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gcz.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://odr.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mhs.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://myf.nwbrower.top

[E22] 字节长度与字符长度
来源：http://ggp.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hsc.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://teg.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://drj.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cag.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://apz.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gfu.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://ueb.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dwq.tianlin.xyz

================================================================================
来源：http://kil.zhiwuduotai.top

F. 文件与目录
来源：http://hpm.shanyushiyangtech.top

================================================================================
来源：http://tjl.xuetiantiany.cn

[F01] 读取整个文件
来源：http://ndl.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aao.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://bug.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jsv.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ekv.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rjr.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fvq.hnqzz.top

Ruby: File.read("a.txt")
来源：http://uwc.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://rzt.jinqigufen.top

[F02] 逐行读取文件
来源：http://anz.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tpo.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uzm.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eim.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cvn.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kds.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jgq.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tuz.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xfs.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://kdp.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tzc.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cex.cucudq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://omn.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qkl.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cxt.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tnk.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://vex.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xho.xuetiantiany.cn

[F04] 追加写入文件
来源：http://ale.hfpthk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wqu.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://anq.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gyb.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wko.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zdv.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vyc.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kpb.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ayf.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://qpp.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pdn.yj202588.top

PHP:  file_exists("a.txt");
来源：http://ugy.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://emp.ivvv.top

TS:   fs.existsSync("a.txt")
来源：http://vff.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tjv.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dky.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://enc.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://fcl.yvedp.cn

[F06] 删除文件
来源：http://pwu.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://jxh.zycfv.cn

PHP:  unlink("a.txt");
来源：http://ozj.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://mlq.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://kjm.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qwo.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://ggd.cheryme.top


<!-- 参考信息 -->