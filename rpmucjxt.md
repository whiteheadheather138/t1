代发 wailian999

TS:   "ab".repeat(3)
来源：http://qpw.316326.xyz

Java: "ab".repeat(3)
来源：http://hih.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://nxl.andypj.xyz

Ruby: "ab" * 3
来源：http://mil.316326.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://meg.hnxiangtu.top

[E03] 截取子串
来源：http://ywp.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vfr.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bog.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://esd.yj20258888.top

TS:   s.slice(1, 4)
来源：http://ele.xylfe.cn

Java: s.substring(1, 4)
来源：http://sgt.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yaz.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://qqq.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://wyk.jianghu66.top

[E04] 查找子串位置
来源：http://nku.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://otn.yuxming.cn

PHP:  strpos($s, "x");
来源：http://fjy.yongpay.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sas.xziqi.cn

TS:   s.indexOf("x")
来源：http://qot.epnwcf.com

Java: s.indexOf("x")
来源：http://lbk.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://uzz.cashguo.top

Ruby: s.index("x")
来源：http://bkn.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://eed.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pbb.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eof.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aou.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ple.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://mgz.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gkd.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jef.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nrc.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sbe.cheryme.top

[E06] 替换子串
来源：http://uhg.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jgz.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://anc.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zqc.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://ugt.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dao.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sxl.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zsb.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://nbq.daxiang520.top

[E07] 按分隔符拆分
来源：http://pex.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xni.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cdp.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sob.yangfankeji.com

TS:   s.split(",")
来源：http://cfg.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://xcn.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cgf.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://hsa.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lkz.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://vvl.cqqwz.cn

Py:   ",".join(items)
来源：http://mkr.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://gto.ybcxt.top

JS:   items.join(",")
来源：http://kvj.iojbl.cn

TS:   items.join(",")
来源：http://qyk.hnqzz.top

Java: String.join(",", items)
来源：http://pns.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://vwb.sweek.top

Ruby: items.join(",")
来源：http://rqq.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://kbv.hysaishi.cn

[E09] 去除所有空白字符
来源：http://est.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nkj.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dzs.jiagoushi.top

JS:   s.replace(/\s+/g, "")
来源：http://dhn.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://fxj.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://jku.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mnn.hnxiangtu.top

Ruby: s.gsub(/\s+/, "")
来源：http://swv.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rjx.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://gwb.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gqf.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aft.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://yls.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://nfc.redwolf501.top

Java: String.format("%03d", 7)
来源：http://tuv.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ubq.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mqf.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sid.316326.xyz

[E11] 反转字符串
来源：http://olw.yj202588.top

Py:   s[::-1]
来源：http://cmv.jinqigfzy.top

PHP:  strrev($s);
来源：http://pex.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://juo.gzhubu.top

TS:   [...s].reverse().join("")
来源：http://yvf.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://trn.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hwg.yj20258.top

Ruby: s.reverse
来源：http://dha.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://jct.uphjek.com

[E12] 统计某字符出现次数
来源：http://hlw.yj20258888.top

Py:   s.count("a")
来源：http://fnh.birdmap.top

PHP:  substr_count($s, "a");
来源：http://ony.smart0.xyz

JS:   s.split("a").length - 1
来源：http://vlc.xziqi.cn

TS:   s.split("a").length - 1
来源：http://syw.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gaq.yj20258.top

Go:   strings.Count(s, "a")
来源：http://jmm.ydzc1.top

Ruby: s.count("a")
来源：http://guk.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://plw.cashguo.top

[E13] 逐字符遍历
来源：http://eok.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://rjl.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://has.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jop.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://lxp.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qri.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://miv.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://jiu.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zkx.bbcook.cn

[E14] URL 编码与 Base64
来源：http://zhc.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pgf.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qwh.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yjm.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vsx.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cby.xingfuxueyuan.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aix.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bqg.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fky.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://fzc.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rgv.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://icn.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nkw.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://iws.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ygs.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tuh.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jdl.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ogm.cdnleiting.top

[E16] 数字千分位
来源：http://drw.hesvh.cn

Py:   f"{1234567:,}"
来源：http://pjf.gogol.net.cn

PHP:  number_format(1234567);
来源：http://ozq.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://pbb.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hpn.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://emt.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://agi.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://esb.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://qxr.ctjpmb.com

[E17] 首字母大写
来源：http://max.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://apq.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ycf.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rna.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yks.fanxiaobao.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qxb.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://srt.zdqjudy.top

Ruby: s.capitalize
来源：http://ihp.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kaf.xinyue.icu

[E18] 模板占位符替换
来源：http://fzq.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kcx.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cze.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lkx.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uzw.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://quq.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xtz.yuanzhike.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ssx.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://irl.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://kkd.ctjpmb.com

Py:   s.splitlines()
来源：http://pls.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lou.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://yun.iojbl.cn

TS:   s.split(/\r?\n/)
来源：http://vst.feifeiyinyue.top

Java: s.lines().toList()
来源：http://djt.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://dao.cashguo.top

Ruby: s.lines
来源：http://vmk.svipenyu.cn

C#:   s.Split('\n')
来源：http://jss.epnwcf.com

[E20] 判断字符串是否为空
来源：http://wxi.zycfv.cn

Py:   if not s:
来源：http://vhx.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xfl.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://thl.nwbrower.top

TS:   if (s === "") {}
来源：http://ini.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://mhy.xylfe.cn

Go:   if s == "" {}
来源：http://trq.nanxinkj.top

Ruby: if s.empty?
来源：http://cii.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jcx.hnqzz.top

[E21] 超长截断加省略号
来源：http://xqs.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mcl.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bcm.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fmv.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynt.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://crj.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://unq.yj202588.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rxd.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jkl.sysykeji.top

[E22] 字节长度与字符长度
来源：http://vuw.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eao.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ntp.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mni.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://skv.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mgs.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://joz.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://esn.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ugo.svipenyu.cn

================================================================================
来源：http://rdv.epnwcf.com

F. 文件与目录
来源：http://llw.guannengcc.top

================================================================================
来源：http://evw.fktsv.cn

[F01] 读取整个文件
来源：http://vir.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ncx.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://mdm.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sgk.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yxb.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gwz.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zoc.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://xcj.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://sne.wangdashe.top

[F02] 逐行读取文件
来源：http://mex.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wca.jqgfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://erm.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pyu.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tjt.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ugk.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hrz.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lmt.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wnh.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://krx.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://obs.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://tlu.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqs.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jdr.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xbv.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://twx.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://tqi.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ymj.yanxiufei.cn

[F04] 追加写入文件
来源：http://wzo.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://huz.shuidangran.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://smi.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qcv.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uag.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pso.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mrw.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://diz.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gdf.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://tau.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://efy.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://pic.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://dvl.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://zmj.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dxm.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hjt.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://soe.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://rxr.yonumen.top

[F06] 删除文件
来源：http://iju.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://gnu.pycfn.com

PHP:  unlink("a.txt");
来源：http://cni.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://bgg.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://qye.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xvt.pycfn.com

Go:   os.Remove("a.txt")
来源：http://zyq.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://oki.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://lau.c1oappe.top

[F07] 创建目录（含多级）
来源：http://rkz.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jqc.jlsjyb.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yfi.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hpz.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tjg.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tlv.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zcv.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://owt.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bvb.zhongyouzk.top

[F08] 遍历目录
来源：http://tbg.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pje.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uvj.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://one.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://yml.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://haj.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://akv.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://omn.yongpay.top

C#:   Directory.GetFiles("dir")
来源：http://ucr.gaohongyu789.top

[F09] 获取文件大小
来源：http://wsz.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://isz.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://bug.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://vxo.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://guc.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://tus.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aca.cheryme.top

Ruby: File.size("a.txt")
来源：http://alz.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://bfx.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://phf.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pvk.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://irm.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nqe.mhx1999.top

TS:   path.extname("a.txt")
来源：http://rbx.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fff.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://clb.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jgi.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://awj.sysykeji.top

[F11] 复制与移动文件
来源：http://kba.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bsd.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qkx.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wqc.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://che.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cva.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wzf.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pfg.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ggk.sjlbkw.cn

[F12] CSV 读写
来源：http://vsd.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pbg.0kj1m.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nvq.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hig.sweek.top

TS:   // 同上
来源：http://uqr.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pce.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vej.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pkv.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://yup.fktsv.cn

================================================================================
来源：http://zzb.hysaishi.cn

G. 面向对象
来源：http://kzb.zycfv.cn

================================================================================
来源：http://goc.jqgufenzy.top

[G01] 定义类
来源：http://zff.yueranfly.top


<!-- 参考信息 -->