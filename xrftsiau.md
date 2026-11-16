代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://cuk.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://dcl.yj202588.top

JS:   arr.join(", ")
来源：http://vkp.zdqjudy.top

TS:   arr.join(", ")
来源：http://mck.xziqi.cn

Java: String.join(", ", list)
来源：http://qqq.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://doj.shuidangran.top

Ruby: arr.join(", ")
来源：http://kyn.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://otm.hongshengwenyu.top

================================================================================
来源：http://imm.quarkkingdee.top

E. 字符串处理
来源：http://lqq.hcnkem.com

================================================================================
来源：http://bqn.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://yxl.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nvu.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mst.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hxj.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qkk.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jlt.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yko.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ada.aibaodan.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jlr.9152youxi.cn

[E02] 重复字符串
来源：http://onz.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://cqk.jinqigfzy.top

PHP:  str_repeat("ab", 3);
来源：http://evw.yonumen.top

JS:   "ab".repeat(3)
来源：http://twp.pycfn.com

TS:   "ab".repeat(3)
来源：http://ege.ydzc1.top

Java: "ab".repeat(3)
来源：http://phy.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://byo.ehwqpu.com

Ruby: "ab" * 3
来源：http://avb.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://che.hfpthk.cn

[E03] 截取子串
来源：http://egi.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lcb.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gtb.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://exf.ybcxt.top

TS:   s.slice(1, 4)
来源：http://ynr.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://bqt.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://smo.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://rtu.cashguo.top

C#:   s.Substring(1, 3)
来源：http://jkh.hnxiangtu.top

[E04] 查找子串位置
来源：http://hmf.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://noi.fengsongda.top

PHP:  strpos($s, "x");
来源：http://ffx.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ypj.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://mcj.bjfxy.top

Java: s.indexOf("x")
来源：http://yef.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://prd.tianlin.xyz

Ruby: s.index("x")
来源：http://knk.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://oha.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xsk.zycfv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tmg.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ocj.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wtw.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uxk.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://trn.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wuj.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xys.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gey.yj202588.top

[E06] 替换子串
来源：http://lhs.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://emy.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://jcx.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://icq.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://wjq.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eyo.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sts.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iki.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://tjq.yangfankeji.com

[E07] 按分隔符拆分
来源：http://bqx.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mhc.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yle.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gkp.fanxiaobao.xyz

TS:   s.split(",")
来源：http://mmx.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://ltd.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mzo.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://ipg.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yrz.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://bns.cucudq.cn

Py:   ",".join(items)
来源：http://zrr.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://tdz.hcnkem.com

JS:   items.join(",")
来源：http://utv.ehwqpu.com

TS:   items.join(",")
来源：http://xqd.quarkkingdee.top

Java: String.join(",", items)
来源：http://clg.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://uws.smart0.xyz

Ruby: items.join(",")
来源：http://oog.yangfankeji.com

C#:   string.Join(",", items)
来源：http://hho.hesvh.cn

[E09] 去除所有空白字符
来源：http://sxv.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bxv.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sye.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://jmg.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://hms.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://voe.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uvo.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://wcb.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sko.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://due.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uwx.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yaj.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://ddh.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://zpi.cashguo.top

Java: String.format("%03d", 7)
来源：http://ecy.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nqd.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jat.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://drl.316326.xyz

[E11] 反转字符串
来源：http://guf.daxiang520.top

Py:   s[::-1]
来源：http://vpq.yuxming.cn

PHP:  strrev($s);
来源：http://yua.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://nto.tarul.cn

TS:   [...s].reverse().join("")
来源：http://eha.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jkw.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pmq.yj20258888.top

Ruby: s.reverse
来源：http://lbd.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://qhj.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://zvg.daria6918.cn

Py:   s.count("a")
来源：http://lyu.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://uyd.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://ipl.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://zxp.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uch.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://ksy.yonumen.top

Ruby: s.count("a")
来源：http://lfp.yanxiufei.cn

C#:   s.Count(c => c == 'a')
来源：http://ylx.vehdjk.com

[E13] 逐字符遍历
来源：http://ibh.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://inz.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ugb.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://bkh.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://utz.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dfn.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kut.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://doj.nanxinkj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kfm.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://zjk.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dlm.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gux.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bcp.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://adn.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hec.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mdt.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eil.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ucd.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://uid.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://rro.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eey.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sce.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://nyu.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://flh.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ivb.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rkd.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://opq.zhiwuduotai.top

[E16] 数字千分位
来源：http://fpe.smart0.xyz

Py:   f"{1234567:,}"
来源：http://pre.316326.xyz

PHP:  number_format(1234567);
来源：http://oci.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jaf.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wyw.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ddv.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pax.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qyo.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://ico.daxiang520.top

[E17] 首字母大写
来源：http://edy.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qlz.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ftt.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oei.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bji.zhongyouzk.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nvf.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zzs.chenzaomai.com

Ruby: s.capitalize
来源：http://tfw.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qts.aibaodan.cn

[E18] 模板占位符替换
来源：http://sxt.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wnj.xziqi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ges.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mmp.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://fzx.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vpm.yj20258888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bsf.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yfk.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aif.gzhubu.top

[E19] 多行文本按行拆分
来源：http://amn.quarkkingdee.top

Py:   s.splitlines()
来源：http://gvx.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vld.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://lno.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://cxm.gzhubu.top

Java: s.lines().toList()
来源：http://nqg.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://iqq.nanxinkj.top

Ruby: s.lines
来源：http://xfp.yongpay.top

C#:   s.Split('\n')
来源：http://hgm.sysykeji.top

[E20] 判断字符串是否为空
来源：http://lqi.jinqigufen.top

Py:   if not s:
来源：http://spe.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rcv.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fwr.chenlongwang.top

TS:   if (s === "") {}
来源：http://evo.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://hxz.shangyingyoupin.top

Go:   if s == "" {}
来源：http://vni.0kj1m.cn

Ruby: if s.empty?
来源：http://gzn.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dwj.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://pxc.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uzf.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://psp.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xyn.ppjwa.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bnc.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://twf.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://lai.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kzu.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://alt.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://zdk.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pfe.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kat.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gzn.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ihj.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rmg.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://skk.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://oyi.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gss.chenzaomai.com

================================================================================
来源：http://vko.tarul.cn

F. 文件与目录
来源：http://uvq.ehwqpu.com

================================================================================
来源：http://hki.cucudq.cn

[F01] 读取整个文件
来源：http://nkt.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://osg.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://rbx.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yia.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zok.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sbw.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nst.smart0.xyz

Ruby: File.read("a.txt")
来源：http://dqo.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://bjt.redwolf501.top

[F02] 逐行读取文件
来源：http://hsw.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://apt.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hbt.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xzv.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://heo.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jfx.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tpp.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qgh.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uxl.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://bku.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dua.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vty.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nhm.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zag.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lyw.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gkj.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://nxx.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oko.yj202588.top

[F04] 追加写入文件
来源：http://jjt.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pxi.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://siu.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://esa.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kfu.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zkh.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hxh.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bxh.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ifp.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://lis.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yaq.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://fub.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://ese.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://ksv.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ske.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uud.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://dcj.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://onw.wangdashe.top

[F06] 删除文件
来源：http://fba.daxiang520.top

Py:   os.remove("a.txt")
来源：http://amt.ctjpmb.com

PHP:  unlink("a.txt");
来源：http://rhw.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://txz.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dpe.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zvr.sweek.top

Go:   os.Remove("a.txt")
来源：http://rbp.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://jaz.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://bxx.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://inb.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://guj.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bwi.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://txd.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hoj.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bwa.zdqjudy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rti.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iar.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zjp.vqdsnc.cn

[F08] 遍历目录
来源：http://rvp.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qqd.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://juq.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://ovr.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://zrn.ybcxt.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://snq.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vbu.daria6918.cn

Ruby: Dir.children("dir")
来源：http://qgc.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://gpp.c1oappe.top

[F09] 获取文件大小
来源：http://dnn.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://tfp.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://sgw.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://moa.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://syq.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://jtk.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://otx.52xcode.cn

Ruby: File.size("a.txt")
来源：http://qfk.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://bwd.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://bbj.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hyk.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xcm.yj202588.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xfi.yfazqb.com

TS:   path.extname("a.txt")
来源：http://uhd.zhijiandao.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mbb.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uxp.tarul.cn


<!-- 参考信息 -->