代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rxs.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zjf.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://yiy.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fzj.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bye.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lop.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aix.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zcs.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hwc.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wgy.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ghn.gogol.net.cn

[D26] 数组转字符串
来源：http://lof.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://qbf.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://gin.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://fie.yvedp.cn

TS:   arr.join(", ")
来源：http://ong.chenzaomai.com

Java: String.join(", ", list)
来源：http://lac.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://dih.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://ehk.fktsv.cn

C#:   string.Join(", ", list)
来源：http://use.jinghuilouyu.cn

================================================================================
来源：http://pru.snrcjt.cn

E. 字符串处理
来源：http://wev.pengpengdd.cyou

================================================================================
来源：http://css.aizwys.cn

[E01] 拼接字符串
来源：http://luv.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hus.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fos.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gxi.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://udt.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dzz.daxiang520.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://myf.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ftu.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eku.jqgfzy.top

[E02] 重复字符串
来源：http://cxc.yonumen.top

Py:   "ab" * 3
来源：http://wgn.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://luu.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://dov.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://fqy.gogol.net.cn

Java: "ab".repeat(3)
来源：http://mod.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://ptx.guannengcc.top

Ruby: "ab" * 3
来源：http://rjp.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rod.0kj1m.cn

[E03] 截取子串
来源：http://ymn.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ymj.dashuyun.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xih.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hlt.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://icp.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://fro.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sht.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rmy.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://xgb.hnqzz.top

[E04] 查找子串位置
来源：http://ybu.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://bxh.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://ypm.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kfg.jianghu66.top

TS:   s.indexOf("x")
来源：http://vus.0kj1m.cn

Java: s.indexOf("x")
来源：http://uby.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://her.meibo888.top

Ruby: s.index("x")
来源：http://fpl.ybcxt.top

C#:   s.IndexOf("x")
来源：http://ulk.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ysy.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ogt.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pfr.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egy.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mtz.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yhk.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ezt.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sap.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tsy.uphjek.com

[E06] 替换子串
来源：http://otf.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xob.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://tnh.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cgg.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://ouw.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xyv.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zkh.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iui.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://tzk.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://oyv.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yka.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jcb.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://uad.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://ecu.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://fdk.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://avm.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://nfn.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bnc.tarul.cn

[E08] 数组按分隔符合并
来源：http://vkj.yj202588.top

Py:   ",".join(items)
来源：http://hmn.fktsv.cn

PHP:  implode(",", $items);
来源：http://nol.316326.xyz

JS:   items.join(",")
来源：http://kyu.birdmap.top

TS:   items.join(",")
来源：http://brw.jqgufenzy.top

Java: String.join(",", items)
来源：http://gnd.shangyingyoupin.top

Go:   strings.Join(items, ",")
来源：http://ynq.bjfxy.top

Ruby: items.join(",")
来源：http://jxe.guannengcc.top

C#:   string.Join(",", items)
来源：http://yuj.guannengcc.top

[E09] 去除所有空白字符
来源：http://jsj.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hnt.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://igk.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://nuz.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://prv.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://kpo.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qnv.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yeg.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://shx.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://cqf.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pyp.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dad.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://rpb.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://jno.daria6918.cn

Java: String.format("%03d", 7)
来源：http://zfa.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xmw.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dym.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uyy.mhx1999.top

[E11] 反转字符串
来源：http://afv.hnqzz.top

Py:   s[::-1]
来源：http://nvr.yongpay.top

PHP:  strrev($s);
来源：http://lrh.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://rnl.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://tgp.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sbk.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://mlk.yangfankeji.com

Ruby: s.reverse
来源：http://ret.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://kbb.52xcode.cn

[E12] 统计某字符出现次数
来源：http://wrf.yfazqb.com

Py:   s.count("a")
来源：http://dnl.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://xnf.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://rpu.fktsv.cn

TS:   s.split("a").length - 1
来源：http://hol.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nlq.yueranfly.top

Go:   strings.Count(s, "a")
来源：http://hxd.pengpengdd.cyou

Ruby: s.count("a")
来源：http://cgj.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://ywz.jyoumei.cn

[E13] 逐字符遍历
来源：http://qxt.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://zte.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uwp.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iax.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gok.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zdl.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zmw.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xwy.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://efy.yueranfly.top

[E14] URL 编码与 Base64
来源：http://tgi.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dbc.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rfs.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lwm.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jzv.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xbc.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://quw.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jkb.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xdd.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://onk.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zio.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qnw.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fsm.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://saa.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ehi.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yhf.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kqe.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zpy.iojbl.cn

[E16] 数字千分位
来源：http://pnx.daxiang520.top

Py:   f"{1234567:,}"
来源：http://bjm.wangdashe.top

PHP:  number_format(1234567);
来源：http://nbm.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fcp.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xwg.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qaf.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ywj.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jet.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://jlg.jiagoushi.top

[E17] 首字母大写
来源：http://qxf.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kup.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://dsl.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jet.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://acg.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qbm.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cnl.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://xbv.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://djc.yj20258.top

[E18] 模板占位符替换
来源：http://ycf.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cqp.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tvi.aizwys.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rtu.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fii.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pci.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://klt.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nkj.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ldl.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://zzc.hysaishi.cn

Py:   s.splitlines()
来源：http://ppz.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://orv.yuanzhike.top

JS:   s.split(/\r?\n/)
来源：http://fqm.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://fhm.vqdsnc.cn

Java: s.lines().toList()
来源：http://uat.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://bdy.gaohongyu789.top

Ruby: s.lines
来源：http://wct.tarul.cn

C#:   s.Split('\n')
来源：http://nxz.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://vof.chenlongwang.top

Py:   if not s:
来源：http://aih.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://alr.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dnb.pycfn.com

TS:   if (s === "") {}
来源：http://ogn.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://ofn.jyoumei.cn

Go:   if s == "" {}
来源：http://lia.yfazqb.com

Ruby: if s.empty?
来源：http://xou.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aef.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://zso.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://onn.fktsv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nck.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qjg.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ejo.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://plx.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://lyz.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yyu.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sub.wangshuangyany.cn

[E22] 字节长度与字符长度
来源：http://xvu.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://izs.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dsa.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ieo.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sar.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jxe.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mhe.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://tyu.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://den.bbcook.cn

================================================================================
来源：http://ylz.yj202588.top

F. 文件与目录
来源：http://glg.xziqi.cn

================================================================================
来源：http://lor.hnqzz.top

[F01] 读取整个文件
来源：http://att.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bld.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://pow.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://glo.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vvl.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bhd.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xap.hcnkem.com

Ruby: File.read("a.txt")
来源：http://rfa.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://gqd.nanxuanxn.top

[F02] 逐行读取文件
来源：http://xeh.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vnk.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://srf.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ilh.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://evu.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mya.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oou.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dzn.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rvb.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://iqy.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vph.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mai.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hfy.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xit.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://crl.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lul.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://gjp.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jvk.yongpay.top

[F04] 追加写入文件
来源：http://wyl.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qyz.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ycs.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ybn.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kua.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bre.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bwh.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nxi.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gzo.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://qsp.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://duv.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://esz.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://atl.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://zps.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ule.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gbq.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://tww.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://una.pycfn.com

[F06] 删除文件
来源：http://fqa.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://oxd.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://kqc.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://mql.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zyq.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ltb.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://rxe.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://ned.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://bdc.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://fsv.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ivy.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xcz.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xle.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tao.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kdn.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ogb.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sjn.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eig.fengsongda.top

[F08] 遍历目录
来源：http://ybz.hywenlv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xag.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eae.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://cyn.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://klj.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wdg.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kku.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://nrg.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://dvq.yfazqb.com

[F09] 获取文件大小
来源：http://pzk.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://wiq.guannengcc.top

PHP:  filesize("a.txt");
来源：http://vhg.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://cno.yongpay.top


<!-- 参考信息 -->