代发 wailian999

================================================================================
来源：http://hsp.ybcxt.top

E. 字符串处理
来源：http://lqr.316326.xyz

================================================================================
来源：http://htz.aibaodan.cn

[E01] 拼接字符串
来源：http://ynn.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://psy.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dya.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sqm.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jjl.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vam.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lzg.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://osa.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hlw.xuetiantiany.cn

[E02] 重复字符串
来源：http://ipe.gzhubu.top

Py:   "ab" * 3
来源：http://qcn.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://trx.316326.xyz

JS:   "ab".repeat(3)
来源：http://kwi.daxiang520.top

TS:   "ab".repeat(3)
来源：http://zfa.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://zmk.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://vhe.ppjwa.cn

Ruby: "ab" * 3
来源：http://pkv.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pum.gzhubu.top

[E03] 截取子串
来源：http://hfs.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dcs.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pti.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tom.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://knr.xziqi.cn

Java: s.substring(1, 4)
来源：http://arj.nanxinkj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://stw.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://fqs.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://tap.feifeiyinyue.top

[E04] 查找子串位置
来源：http://ozf.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://jje.birdmap.top

PHP:  strpos($s, "x");
来源：http://ied.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iew.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://dth.zhixingplan.top

Java: s.indexOf("x")
来源：http://kiv.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://lmj.316326.xyz

Ruby: s.index("x")
来源：http://jwi.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://zsi.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pkt.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mqf.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wrt.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://crz.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zle.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tbc.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hmd.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xma.nanxuanxn.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xso.9152youxi.cn

[E06] 替换子串
来源：http://hyb.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xyz.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://swt.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ppf.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://wur.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://znl.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yrz.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://srf.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://sdi.xziqi.cn

[E07] 按分隔符拆分
来源：http://tzs.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jzm.hywenlv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vpz.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://bnv.ybcxt.top

TS:   s.split(",")
来源：http://ajh.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oas.zhijiandao.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tny.haohaochexian.top

Ruby: s.split(",");  s.split
来源：http://bqn.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hxk.epnwcf.com

[E08] 数组按分隔符合并
来源：http://rjg.daria6918.cn

Py:   ",".join(items)
来源：http://ktn.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://yli.xziqi.cn

JS:   items.join(",")
来源：http://iid.chenlongwang.top

TS:   items.join(",")
来源：http://fya.yanxiufei.cn

Java: String.join(",", items)
来源：http://crt.pycfn.com

Go:   strings.Join(items, ",")
来源：http://ylg.cucudq.cn

Ruby: items.join(",")
来源：http://kvz.shzxlz.cn

C#:   string.Join(",", items)
来源：http://prk.xinyue.icu

[E09] 去除所有空白字符
来源：http://hao.xylfe.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wwj.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bqe.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://mqi.ydjk.org.cn

TS:   s.replace(/\s+/g, "")
来源：http://fic.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://ite.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rbd.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://lkt.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xot.xziqi.cn

[E10] 左侧补零 / 定长填充
来源：http://tlp.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nym.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hhe.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://xgj.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://sol.xinyue.icu

Java: String.format("%03d", 7)
来源：http://uie.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://bsc.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://glk.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hsr.guowangkeji.top

[E11] 反转字符串
来源：http://nmh.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://ulg.wangshuangyany.cn

PHP:  strrev($s);
来源：http://daq.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://cxz.yonumen.top

TS:   [...s].reverse().join("")
来源：http://jai.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zvy.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pph.pengpengdd.cyou

Ruby: s.reverse
来源：http://kwe.jiagoushi.top

C#:   new string(s.Reverse().ToArray())
来源：http://ngk.wangdashe.top

[E12] 统计某字符出现次数
来源：http://tww.redwolf501.top

Py:   s.count("a")
来源：http://ydp.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://pgj.yonumen.top

JS:   s.split("a").length - 1
来源：http://pde.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://cfn.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://trn.birdmap.top

Go:   strings.Count(s, "a")
来源：http://pup.hammf.cn

Ruby: s.count("a")
来源：http://tru.zhengqikj.top

C#:   s.Count(c => c == 'a')
来源：http://ojm.bjfxy.top

[E13] 逐字符遍历
来源：http://ive.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://fbe.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qch.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://czw.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iue.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kop.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hlu.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pwe.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mkb.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://vka.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://emm.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rpy.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ggt.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kgn.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fzp.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mtu.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bvo.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jnu.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://qxh.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://umx.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://raa.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ebv.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rhh.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bkz.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://udn.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jzy.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bhn.ehwqpu.com

[E16] 数字千分位
来源：http://twa.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://rux.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://pfe.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://suf.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zrb.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jpd.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nwv.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mkh.sjlbkw.cn

C#:   1234567.ToString("N0")
来源：http://dmk.xziqi.cn

[E17] 首字母大写
来源：http://psi.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://htg.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sxh.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eqb.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yal.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vwh.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qpi.chenlongwang.top

Ruby: s.capitalize
来源：http://ous.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iqx.gzhubu.top

[E18] 模板占位符替换
来源：http://tiv.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kgr.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://omr.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://epw.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ono.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://djo.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zcn.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zjv.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ivq.9152youxi.cn

[E19] 多行文本按行拆分
来源：http://kgh.yj20258888.top

Py:   s.splitlines()
来源：http://qwl.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wxa.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://clj.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://mci.hfpthk.cn

Java: s.lines().toList()
来源：http://mwf.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://ljx.yangfankeji.com

Ruby: s.lines
来源：http://vii.cqqwz.cn

C#:   s.Split('\n')
来源：http://amf.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://moj.yangfankeji.com

Py:   if not s:
来源：http://knx.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iga.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://owe.cdnleiting.top

TS:   if (s === "") {}
来源：http://qxd.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://jnb.hfpthk.cn

Go:   if s == "" {}
来源：http://pxy.jlsjyb.cn

Ruby: if s.empty?
来源：http://ifn.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jzx.yangfankeji.com

[E21] 超长截断加省略号
来源：http://cap.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://quu.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://idh.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://spj.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iux.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tym.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://tku.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rfx.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qye.fktsv.cn

[E22] 字节长度与字符长度
来源：http://fgb.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://flb.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sxq.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lso.yonumen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyq.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ffx.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ptd.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://uam.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oae.iojbl.cn

================================================================================
来源：http://mmf.tianlin.xyz

F. 文件与目录
来源：http://xvs.nanxuanxn.top

================================================================================
来源：http://yxu.cheryme.top

[F01] 读取整个文件
来源：http://uxw.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hyw.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://jlz.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kjq.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ofn.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cdh.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://olh.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://gpe.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://zpc.yuanzhike.top

[F02] 逐行读取文件
来源：http://jfk.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://djl.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zsn.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lrj.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hns.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://maa.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dwp.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vyi.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://spj.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://pds.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jgc.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xdh.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pnx.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jol.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bch.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ogb.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://gnc.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tag.fehbvm.com

[F04] 追加写入文件
来源：http://zun.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nky.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ydi.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vwb.shanyushiyangtech.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://slw.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://paf.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wou.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lzv.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tvh.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://uik.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oka.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://eef.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://cxy.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://lhb.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://adv.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://olg.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://usx.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://aix.dashuyun.cn

[F06] 删除文件
来源：http://wbb.ivvv.top

Py:   os.remove("a.txt")
来源：http://roq.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://zrz.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://mde.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://jre.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zaz.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://qpp.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://nqo.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://zaa.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://kuc.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wzh.0kj1m.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uws.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jpn.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tqt.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://shj.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nqg.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pwy.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qmz.yonumen.top

[F08] 遍历目录
来源：http://pjb.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://syc.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fla.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://hqe.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://wrr.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vzu.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://gbj.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://fbk.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://otx.fzhhl.top

[F09] 获取文件大小
来源：http://dqc.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://pby.tanke756.top

PHP:  filesize("a.txt");
来源：http://jxj.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://mps.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://ezk.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://fyy.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vwf.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://byn.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://onm.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://yqp.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lvy.jiagoushi.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jis.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tfm.ivvv.top

TS:   path.extname("a.txt")
来源：http://gle.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vvc.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://odv.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://igf.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sds.hnxiangtu.top

[F11] 复制与移动文件
来源：http://hmk.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mah.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://icx.yanxiufei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cas.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ywm.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hdl.yvedp.cn


<!-- 参考信息 -->