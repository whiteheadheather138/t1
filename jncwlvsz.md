代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kud.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://bve.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jpd.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jgc.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vch.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bws.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cil.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://adu.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tcf.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vzv.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://snz.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://quv.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qzd.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lsz.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xbu.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dva.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zpy.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dgp.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cza.uphjek.com

[D26] 数组转字符串
来源：http://dbi.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://fqh.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://yvy.vqdsnc.cn

JS:   arr.join(", ")
来源：http://drr.andypj.xyz

TS:   arr.join(", ")
来源：http://clx.zdbjq.cn

Java: String.join(", ", list)
来源：http://efn.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://tnr.redwolf501.top

Ruby: arr.join(", ")
来源：http://rgw.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://qra.aibaodan.cn

================================================================================
来源：http://ugh.fehbvm.com

E. 字符串处理
来源：http://vhj.gotoacloud.top

================================================================================
来源：http://ecp.jianghu66.top

[E01] 拼接字符串
来源：http://ydl.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lie.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tnc.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kcf.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fvw.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vwz.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yjd.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ywb.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yvv.havefunace.top

[E02] 重复字符串
来源：http://jxe.zdbjq.cn

Py:   "ab" * 3
来源：http://tqp.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://hvr.jianghu66.top

JS:   "ab".repeat(3)
来源：http://ahy.52xcode.cn

TS:   "ab".repeat(3)
来源：http://nio.zdqjudy.top

Java: "ab".repeat(3)
来源：http://ekl.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://yqx.shzxlz.cn

Ruby: "ab" * 3
来源：http://gmr.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hvg.shanyushiyangtech.top

[E03] 截取子串
来源：http://tsn.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aou.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ite.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bwj.yongpay.top

TS:   s.slice(1, 4)
来源：http://wvh.fehbvm.com

Java: s.substring(1, 4)
来源：http://sml.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fyj.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://dgu.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://fmq.yueranfly.top

[E04] 查找子串位置
来源：http://sbe.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://pxm.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://yco.ybcxt.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vxj.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://aem.hnqzz.top

Java: s.indexOf("x")
来源：http://vhd.tanke756.top

Go:   strings.Index(s, "x")
来源：http://vat.jqgfzy.top

Ruby: s.index("x")
来源：http://zeq.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://juy.hammf.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fef.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jik.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yob.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mpr.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bdm.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tdk.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://upm.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fkp.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eir.aibaodan.cn

[E06] 替换子串
来源：http://fcq.vqdsnc.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qdu.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://pla.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hvc.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://jsr.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iaq.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ehb.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wsu.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://enj.epnwcf.com

[E07] 按分隔符拆分
来源：http://aka.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ibf.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kfv.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kam.chenzaomai.com

TS:   s.split(",")
来源：http://arq.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://syj.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ahp.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://qqx.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mze.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://qyh.zhixingplan.top

Py:   ",".join(items)
来源：http://rvs.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://mdb.sweek.top

JS:   items.join(",")
来源：http://cro.fengsongda.top

TS:   items.join(",")
来源：http://osd.yuanzhike.top

Java: String.join(",", items)
来源：http://ban.sxryk.cn

Go:   strings.Join(items, ",")
来源：http://otr.bbcook.cn

Ruby: items.join(",")
来源：http://isy.hysaishi.cn

C#:   string.Join(",", items)
来源：http://tsa.gzhubu.top

[E09] 去除所有空白字符
来源：http://wmo.ivvv.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://efb.hfpthk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tgr.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://ove.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://ghp.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://kqs.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://onw.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://kft.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hef.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://wxe.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wzo.chenjidiqi.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://buo.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://ypp.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://ebt.birdmap.top

Java: String.format("%03d", 7)
来源：http://fgu.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nsc.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gnw.zhaomingkeji.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://phr.jyoumei.cn

[E11] 反转字符串
来源：http://vnk.yuxming.cn

Py:   s[::-1]
来源：http://vgz.daxiang520.top

PHP:  strrev($s);
来源：http://nzi.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://bld.uphjek.com

TS:   [...s].reverse().join("")
来源：http://ywj.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://szr.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://lqa.chenzaomai.com

Ruby: s.reverse
来源：http://lfo.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://ady.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://iop.yvedp.cn

Py:   s.count("a")
来源：http://zzr.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://pau.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://uql.ydzc1.top

TS:   s.split("a").length - 1
来源：http://hfu.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iya.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://szd.xuetiantiany.cn

Ruby: s.count("a")
来源：http://ejx.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://too.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://wyv.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://mxm.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dkv.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ely.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://mzv.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zue.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rge.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yqx.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eai.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://vot.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nij.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://raa.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gjl.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qgn.jinghuilouyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fxa.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ogg.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dfm.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mim.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://ebt.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ooe.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ubx.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mjq.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eot.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zfv.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cbl.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ukx.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pen.haohaochexian.top

[E16] 数字千分位
来源：http://xic.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://dgk.guowangkeji.top

PHP:  number_format(1234567);
来源：http://dju.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yny.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mkx.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vzu.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fdc.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jtp.yj20258.top

C#:   1234567.ToString("N0")
来源：http://rtl.shzxlz.cn

[E17] 首字母大写
来源：http://vlc.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rnb.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://odm.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cic.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rvp.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dms.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://psy.yj20258.top

Ruby: s.capitalize
来源：http://whc.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zmu.birdmap.top

[E18] 模板占位符替换
来源：http://xlb.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rst.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zkj.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cpp.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ngn.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://udl.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wky.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://byw.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gxp.nwbrower.top

[E19] 多行文本按行拆分
来源：http://dul.epnwcf.com

Py:   s.splitlines()
来源：http://nwy.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pxs.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://epi.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://gyx.cqqwz.cn

Java: s.lines().toList()
来源：http://koi.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://jxy.yuxming.cn

Ruby: s.lines
来源：http://ofg.ydzc1.top

C#:   s.Split('\n')
来源：http://ziw.yonumen.top

[E20] 判断字符串是否为空
来源：http://nva.shanyushiyangtech.top

Py:   if not s:
来源：http://rbo.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jqk.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xda.sysykeji.top

TS:   if (s === "") {}
来源：http://fdf.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://kne.hywenlv.cn

Go:   if s == "" {}
来源：http://ngx.xinyue.icu

Ruby: if s.empty?
来源：http://ero.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ogz.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://wvd.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ueh.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uia.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bas.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sip.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://myd.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://fym.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nkw.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zii.chenjidiqi.icu

[E22] 字节长度与字符长度
来源：http://lgy.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xvl.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://isn.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mnb.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://you.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yyl.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pqd.daxiang520.top

Ruby: s.bytesize;  s.length
来源：http://jjd.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pxm.shangyingyoupin.top

================================================================================
来源：http://byd.ctjpmb.com

F. 文件与目录
来源：http://eau.sjlbkw.cn

================================================================================
来源：http://mby.ehwqpu.com

[F01] 读取整个文件
来源：http://pip.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tid.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://xpg.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://byz.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sbo.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://onb.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vgb.shuidangran.top

Ruby: File.read("a.txt")
来源：http://rji.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://otn.hnxiangtu.top

[F02] 逐行读取文件
来源：http://sbe.zhaomingkeji.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cbu.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kuq.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://okq.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ivg.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vik.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wjq.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ybe.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bst.mhx1999.top

[F03] 写入文件（覆盖）
来源：http://oxo.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yuj.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dfu.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pqy.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fwy.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://clm.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ixm.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://nnl.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ffr.jianghu66.top

[F04] 追加写入文件
来源：http://arj.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rga.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rna.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ncz.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sge.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ega.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hwl.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://olm.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xxv.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://qzj.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nml.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://sil.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://ytu.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://rke.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fcz.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hbj.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://yme.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://sac.xinyue.icu

[F06] 删除文件
来源：http://lss.xuanzx.com

Py:   os.remove("a.txt")
来源：http://nhj.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://ows.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://tyf.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wxp.bjfxy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dcs.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://ezz.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://zvw.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://ppx.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://jpm.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ffj.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xdb.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bkk.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vzq.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://beu.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nie.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eup.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bmt.sysykeji.top

[F08] 遍历目录
来源：http://mhf.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lmh.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kcy.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://jyg.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://thu.chenjidiqi.icu


<!-- 参考信息 -->