代发 wailian999

TS:   "ab".repeat(3)
来源：http://mbo.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://yqm.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://obx.svipenyu.cn

Ruby: "ab" * 3
来源：http://dsy.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fgn.jinyuanbaomall.cn

[E03] 截取子串
来源：http://pym.jinghuilouyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xnm.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qnr.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kbv.yj202588.top

TS:   s.slice(1, 4)
来源：http://zoh.vehdjk.com

Java: s.substring(1, 4)
来源：http://nuj.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tex.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://uhz.sweek.top

C#:   s.Substring(1, 3)
来源：http://xhx.snrcjt.cn

[E04] 查找子串位置
来源：http://uid.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://bfa.yangfankeji.com

PHP:  strpos($s, "x");
来源：http://hpv.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gde.zhixingplan.top

TS:   s.indexOf("x")
来源：http://rbk.yj202588.top

Java: s.indexOf("x")
来源：http://xbe.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://kmo.xuetiantiany.cn

Ruby: s.index("x")
来源：http://whc.fktsv.cn

C#:   s.IndexOf("x")
来源：http://vuz.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wzk.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://caj.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wwb.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gne.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hpz.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vty.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fyi.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ofg.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zwh.mhx1999.top

[E06] 替换子串
来源：http://xem.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://chp.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://wnl.feifeiyinyue.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xym.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://zdh.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yjb.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bop.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hka.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://mut.tian-w.cn

[E07] 按分隔符拆分
来源：http://zbv.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bsc.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vrn.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://akx.ehwqpu.com

TS:   s.split(",")
来源：http://nef.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://xjg.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ndl.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://ltf.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wow.hcnkem.com

[E08] 数组按分隔符合并
来源：http://tyi.xylfe.cn

Py:   ",".join(items)
来源：http://wuv.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://oww.wangdashe.top

JS:   items.join(",")
来源：http://ntt.kuanghao11.cn

TS:   items.join(",")
来源：http://tgq.ehwqpu.com

Java: String.join(",", items)
来源：http://ybb.mhx1999.top

Go:   strings.Join(items, ",")
来源：http://jen.daxiang520.top

Ruby: items.join(",")
来源：http://vzi.aizwys.cn

C#:   string.Join(",", items)
来源：http://jsr.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://rmt.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://owk.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nyt.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://ypz.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://sbs.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://clv.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ghw.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://fwh.nwbrower.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lei.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://ngy.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ahs.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dnl.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://dmy.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://bjy.yueranfly.top

Java: String.format("%03d", 7)
来源：http://wrh.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://ktn.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yue.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fcj.jqgufenzy.top

[E11] 反转字符串
来源：http://avo.jinqigfzy.top

Py:   s[::-1]
来源：http://kzq.yuxming.cn

PHP:  strrev($s);
来源：http://odf.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://mpt.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://ugz.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://urx.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aws.xinyue.icu

Ruby: s.reverse
来源：http://kqf.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nla.xuanzx.com

[E12] 统计某字符出现次数
来源：http://swd.chenzaomai.com

Py:   s.count("a")
来源：http://wmn.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://ifk.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://ooy.fktsv.cn

TS:   s.split("a").length - 1
来源：http://tvq.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ixz.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://mka.hysaishi.cn

Ruby: s.count("a")
来源：http://lpv.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://xkq.cdnleiting.top

[E13] 逐字符遍历
来源：http://lpj.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://jtd.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hqy.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qpc.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zso.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yij.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tqe.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jgu.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ifc.pycfn.com

[E14] URL 编码与 Base64
来源：http://osl.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vft.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://hkw.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bwp.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ydk.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vxn.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nyw.zhaomingkeji.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vil.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fkh.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://wll.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://vyn.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gzz.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://noq.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lxs.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://igl.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mdw.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zla.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aao.havefunace.top

[E16] 数字千分位
来源：http://ozs.yj20258.top

Py:   f"{1234567:,}"
来源：http://yff.meibo888.top

PHP:  number_format(1234567);
来源：http://tjw.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zgh.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pab.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fck.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://otm.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yfh.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://psi.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://fen.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bow.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vfa.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zna.gaohongyu789.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jjr.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mji.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ltu.gzhubu.top

Ruby: s.capitalize
来源：http://arw.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zna.meibo888.top

[E18] 模板占位符替换
来源：http://rsy.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jyf.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nbe.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://scq.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oug.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cst.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vel.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xmc.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kcn.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://ess.sxryk.cn

Py:   s.splitlines()
来源：http://wza.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hci.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://wan.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://mlp.dashuyun.cn

Java: s.lines().toList()
来源：http://zxm.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://cwh.yuanzhike.top

Ruby: s.lines
来源：http://ozv.jinqigfzy.top

C#:   s.Split('\n')
来源：http://axn.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://fom.hongshengwenyu.top

Py:   if not s:
来源：http://eko.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vom.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ozv.pycfn.com

TS:   if (s === "") {}
来源：http://swh.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://udw.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://whe.xuetiantiany.cn

Ruby: if s.empty?
来源：http://jlt.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cud.hnqzz.top

[E21] 超长截断加省略号
来源：http://ste.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qad.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hck.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uwf.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://auo.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jmk.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://jsh.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vxw.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tov.hesvh.cn

[E22] 字节长度与字符长度
来源：http://jrq.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://atr.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iqi.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jul.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mkg.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ewr.havefunace.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mdc.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://uje.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://azo.cqqwz.cn

================================================================================
来源：http://exe.xingfuxueyuan.xyz

F. 文件与目录
来源：http://esu.yanxiufei.cn

================================================================================
来源：http://ini.hongshengwenyu.top

[F01] 读取整个文件
来源：http://wmf.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lll.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://pfi.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cii.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gyw.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sbf.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yzt.c1oappe.top

Ruby: File.read("a.txt")
来源：http://izb.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://lqc.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://zgt.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wqu.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zrx.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ioe.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eae.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hmy.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uza.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kwy.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://giq.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://les.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pau.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vhv.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uol.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ggo.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nkf.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lpg.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://vre.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://klp.aizwys.cn

[F04] 追加写入文件
来源：http://sev.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://emg.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rwc.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qia.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tav.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vne.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zbv.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mep.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ndf.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://moj.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hvs.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://iiq.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://dlt.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://tut.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cdq.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zvf.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://cut.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://rjj.yangfankeji.com

[F06] 删除文件
来源：http://fjg.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://wps.sysykeji.top

PHP:  unlink("a.txt");
来源：http://tpw.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://kqc.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://igq.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mnj.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://igf.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://mjx.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://kuw.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://gfw.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zpv.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://drt.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://soq.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://stp.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bzh.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uvf.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oic.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://beq.meibo888.top

[F08] 遍历目录
来源：http://iai.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zqg.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://amk.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://zap.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://nxj.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ude.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://npr.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://aha.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://vlf.pycfn.com

[F09] 获取文件大小
来源：http://pue.hesvh.cn

Py:   os.path.getsize("a.txt")
来源：http://iud.hcnkem.com

PHP:  filesize("a.txt");
来源：http://dom.ppjwa.cn

JS:   fs.statSync("a.txt").size
来源：http://maq.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://gri.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://vpg.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zfy.ydzc1.top

Ruby: File.size("a.txt")
来源：http://ygm.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://xwh.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://kmp.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ylw.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://snd.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ygc.sweek.top

TS:   path.extname("a.txt")
来源：http://ynz.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xzp.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vao.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xww.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://naj.cqqwz.cn

[F11] 复制与移动文件
来源：http://hrl.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xuz.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://itz.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://exd.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pqw.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wbx.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sdu.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iqc.yongpay.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iom.zycfv.cn

[F12] CSV 读写
来源：http://eis.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wmw.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tag.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cel.jinqigfzy.top

TS:   // 同上
来源：http://uph.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zad.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vax.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://clz.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ngo.zdqjudy.top

================================================================================
来源：http://wlu.jlsjyb.cn

G. 面向对象
来源：http://qbg.sufxvd.cn

================================================================================
来源：http://hnm.dianchejie.cn

[G01] 定义类
来源：http://jxr.jlsjyb.cn


<!-- 参考信息 -->