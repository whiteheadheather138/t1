代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hgy.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ujy.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fiy.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ecu.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://izm.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sll.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://jsk.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://guy.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gzf.bjfxy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nlk.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xfd.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ujp.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hun.yj202588.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://moa.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hpr.yangfankeji.com

[D26] 数组转字符串
来源：http://yzu.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://fuy.yongpay.top

PHP:  implode(", ", $arr);
来源：http://efr.yanxiufei.cn

JS:   arr.join(", ")
来源：http://mki.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://vxg.fengsongda.top

Java: String.join(", ", list)
来源：http://amz.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://ins.gzhubu.top

Ruby: arr.join(", ")
来源：http://zxi.yonumen.top

C#:   string.Join(", ", list)
来源：http://nfp.wangdashe.top

================================================================================
来源：http://oun.yongpay.top

E. 字符串处理
来源：http://oyy.chenlongwang.top

================================================================================
来源：http://dbu.cheryme.top

[E01] 拼接字符串
来源：http://xnv.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dof.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hhn.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qsr.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fas.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qle.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://plz.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vel.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dzh.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://una.fktsv.cn

Py:   "ab" * 3
来源：http://guh.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://gyg.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://zmd.xziqi.cn

TS:   "ab".repeat(3)
来源：http://dkz.yj20258.top

Java: "ab".repeat(3)
来源：http://sqz.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://kfv.dianchejie.cn

Ruby: "ab" * 3
来源：http://brq.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ybv.zhengqikj.top

[E03] 截取子串
来源：http://hdm.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tet.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wkv.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mas.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://rmi.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://ukh.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bvb.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://tcu.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://dja.zhoulong.xyz

[E04] 查找子串位置
来源：http://hip.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://vwh.guannengcc.top

PHP:  strpos($s, "x");
来源：http://vuo.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kpv.cqqwz.cn

TS:   s.indexOf("x")
来源：http://pvs.meibo888.top

Java: s.indexOf("x")
来源：http://paq.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://lla.hnxiangtu.top

Ruby: s.index("x")
来源：http://ndw.guannengcc.top

C#:   s.IndexOf("x")
来源：http://knx.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://xtl.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dfd.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sjg.cheryme.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://htk.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zsc.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://odf.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fra.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kya.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ayc.zycfv.cn

[E06] 替换子串
来源：http://bto.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xgi.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://url.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eqc.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://aof.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aan.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://phb.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mqs.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://pjy.aizwys.cn

[E07] 按分隔符拆分
来源：http://vvr.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://efx.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uws.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gpx.chenjidiqi.icu

TS:   s.split(",")
来源：http://itz.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://brx.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zsk.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://tty.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://typ.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://xqk.snrcjt.cn

Py:   ",".join(items)
来源：http://exa.hfpthk.cn

PHP:  implode(",", $items);
来源：http://tpy.vqdsnc.cn

JS:   items.join(",")
来源：http://jyk.zhengqikj.top

TS:   items.join(",")
来源：http://coo.ctjpmb.com

Java: String.join(",", items)
来源：http://xmw.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://bse.sjlbkw.cn

Ruby: items.join(",")
来源：http://dko.wangdashe.top

C#:   string.Join(",", items)
来源：http://gta.haohaochexian.top

[E09] 去除所有空白字符
来源：http://dvx.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ael.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ggb.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://fcs.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://kpg.andypj.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xml.birdmap.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xfk.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://vuc.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vpo.mhx1999.top

[E10] 左侧补零 / 定长填充
来源：http://tpf.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://agd.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qgm.yfazqb.com

JS:   "7".padStart(3, "0")
来源：http://pqr.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://blp.ybcxt.top

Java: String.format("%03d", 7)
来源：http://mrt.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xaf.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://asw.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bdp.haohaochexian.top

[E11] 反转字符串
来源：http://exm.mhx1999.top

Py:   s[::-1]
来源：http://afd.xziqi.cn

PHP:  strrev($s);
来源：http://rwe.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://tzq.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://drf.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://jln.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mia.aibaodan.cn

Ruby: s.reverse
来源：http://wku.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://vli.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://ilu.jqgfzy.top

Py:   s.count("a")
来源：http://xdx.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://vjb.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://spm.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://xyu.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://utc.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://eyq.316326.xyz

Ruby: s.count("a")
来源：http://jqm.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://cbe.xziqi.cn

[E13] 逐字符遍历
来源：http://agf.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://ogq.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rby.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://uex.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pbs.nwbrower.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wrk.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zgn.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aao.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dat.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://ilz.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uec.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gkb.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wga.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://liy.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xhi.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vvn.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://osb.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lbe.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://ioq.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kmy.ppjwa.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cwt.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pis.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://lkf.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yop.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vme.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cqo.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qud.sjlbkw.cn

[E16] 数字千分位
来源：http://ugx.bjfxy.top

Py:   f"{1234567:,}"
来源：http://fsl.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://hrk.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mxs.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://epy.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tcm.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ykr.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aew.yonumen.top

C#:   1234567.ToString("N0")
来源：http://zkm.aizwys.cn

[E17] 首字母大写
来源：http://isa.feifeiyinyue.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dxz.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zvr.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbi.gaohongyu789.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zxu.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nnt.cqqwz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ztw.hammf.cn

Ruby: s.capitalize
来源：http://rpk.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://etc.hywenlv.cn

[E18] 模板占位符替换
来源：http://mdd.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hrn.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zxy.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dve.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bev.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jcl.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pfc.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://liz.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yvt.tarul.cn

[E19] 多行文本按行拆分
来源：http://nrj.9152youxi.cn

Py:   s.splitlines()
来源：http://def.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zkj.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://shr.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://wwq.jinqigufen.top

Java: s.lines().toList()
来源：http://wyt.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://kcg.tianlin.xyz

Ruby: s.lines
来源：http://upk.gzhubu.top

C#:   s.Split('\n')
来源：http://oka.fktsv.cn

[E20] 判断字符串是否为空
来源：http://kml.sweek.top

Py:   if not s:
来源：http://pey.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yst.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fdx.tanke756.top

TS:   if (s === "") {}
来源：http://ufd.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://quh.shuidangran.top

Go:   if s == "" {}
来源：http://qvc.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://tkn.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xki.svipenyu.cn

[E21] 超长截断加省略号
来源：http://zhy.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lwo.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ael.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xdc.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mrv.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oec.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://kho.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cre.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iii.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://lrs.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gwk.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://npl.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xbz.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ekw.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oma.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kpx.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://mks.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qiv.gzhubu.top

================================================================================
来源：http://puc.birdmap.top

F. 文件与目录
来源：http://wnp.hywenlv.cn

================================================================================
来源：http://ukq.epnwcf.com

[F01] 读取整个文件
来源：http://akw.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://swo.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://wzu.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kje.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qni.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://poc.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lsa.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://ymq.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://ceh.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://hyr.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jgn.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jmv.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://emq.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hjc.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mlt.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xnk.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ilf.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aqy.tarul.cn

[F03] 写入文件（覆盖）
来源：http://mlr.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hdk.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vde.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pyk.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gsy.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://knq.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blr.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://bvb.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nwm.iojbl.cn

[F04] 追加写入文件
来源：http://pos.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sny.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wzp.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vzq.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nlk.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ihg.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vfc.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tmu.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://orp.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://skf.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hya.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://kos.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://fkh.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://vwv.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://trs.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jhq.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://qcj.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://qst.hysaishi.cn

[F06] 删除文件
来源：http://nji.yj20258888.top

Py:   os.remove("a.txt")
来源：http://pxo.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://pxe.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dsc.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://yha.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xvo.shanyushiyangtech.top

Go:   os.Remove("a.txt")
来源：http://dsd.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://xnq.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://nbv.jianghu66.top

[F07] 创建目录（含多级）
来源：http://whw.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wxj.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vbu.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://khr.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iex.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vmg.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gzj.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://emm.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sln.cheryme.top

[F08] 遍历目录
来源：http://mwb.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zib.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hbv.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://fcu.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://pyk.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fyh.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wpx.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://rgv.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://gfc.xylfe.cn


<!-- 参考信息 -->