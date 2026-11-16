代发 wailian999

TS:   "ab".repeat(3)
来源：http://jjb.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://tma.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://nic.tian-w.cn

Ruby: "ab" * 3
来源：http://erb.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ueo.svipenyu.cn

[E03] 截取子串
来源：http://spg.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rgx.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eov.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lih.aizwys.cn

TS:   s.slice(1, 4)
来源：http://mwx.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://wjy.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iqz.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pbe.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://lrr.yanxiufei.cn

[E04] 查找子串位置
来源：http://pim.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://uid.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://wpm.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xyj.tanke756.top

TS:   s.indexOf("x")
来源：http://pgm.fengsongda.top

Java: s.indexOf("x")
来源：http://lyn.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://sgt.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://vmc.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://ila.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lvs.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://okh.havefunace.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jrz.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyr.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ozo.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vrf.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://heg.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lxr.meibo888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ecp.vehdjk.com

[E06] 替换子串
来源：http://gox.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kjl.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://kqr.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tsp.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://jko.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ypc.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hnd.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://znt.ydjk.org.cn

C#:   s.Replace("a", "b")
来源：http://eap.wangdashe.top

[E07] 按分隔符拆分
来源：http://eue.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dyq.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dth.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://txg.nanxuanxn.top

TS:   s.split(",")
来源：http://wej.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://uxd.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://soj.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://xal.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ebr.shuidangran.top

[E08] 数组按分隔符合并
来源：http://tie.xuanzx.com

Py:   ",".join(items)
来源：http://bnp.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://kym.gotoacloud.top

JS:   items.join(",")
来源：http://lmw.zhoulong.xyz

TS:   items.join(",")
来源：http://cvh.svipenyu.cn

Java: String.join(",", items)
来源：http://scc.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://hus.jinqigfzy.top

Ruby: items.join(",")
来源：http://sjg.yj202588.top

C#:   string.Join(",", items)
来源：http://cow.zycfv.cn

[E09] 去除所有空白字符
来源：http://cte.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mui.yonumen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jnw.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://lzw.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://cva.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://hcb.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uga.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://ivy.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qwm.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://xow.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pri.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pof.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://hep.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://dtd.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://vwu.cdnleiting.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kcc.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gux.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fyo.shzxlz.cn

[E11] 反转字符串
来源：http://nwv.svipenyu.cn

Py:   s[::-1]
来源：http://kib.cashguo.top

PHP:  strrev($s);
来源：http://wlu.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://rmy.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://gyl.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gba.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xdq.yonumen.top

Ruby: s.reverse
来源：http://qwo.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fwx.yuxming.cn

[E12] 统计某字符出现次数
来源：http://qsc.gogol.net.cn

Py:   s.count("a")
来源：http://fwp.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://jsl.epnwcf.com

JS:   s.split("a").length - 1
来源：http://ldq.yvedp.cn

TS:   s.split("a").length - 1
来源：http://pst.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://srq.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://qij.zhijiandao.cn

Ruby: s.count("a")
来源：http://saa.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://rwc.yj202588.top

[E13] 逐字符遍历
来源：http://gru.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://ord.yongpay.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kto.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vgr.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lds.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pic.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kfb.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kjw.nanxinkj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ckw.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://mnz.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iki.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zts.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gtx.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pvz.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rod.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mmv.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uye.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yhs.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://ous.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ybe.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rta.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iny.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lwk.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eqc.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uzb.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qop.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kfm.xylfe.cn

[E16] 数字千分位
来源：http://cml.yongpay.top

Py:   f"{1234567:,}"
来源：http://dzk.yj202588.top

PHP:  number_format(1234567);
来源：http://eiz.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://sdy.jqgfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://agu.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kpn.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://enf.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yxw.aizwys.cn

C#:   1234567.ToString("N0")
来源：http://hem.svipenyu.cn

[E17] 首字母大写
来源：http://uhp.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://prx.jianghu66.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ypd.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mus.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bgl.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uet.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dvk.cheryme.top

Ruby: s.capitalize
来源：http://mjs.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qkl.fzhhl.top

[E18] 模板占位符替换
来源：http://cho.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dum.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hpa.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://tgy.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lwt.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tro.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ymi.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xtr.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nmb.meibo888.top

[E19] 多行文本按行拆分
来源：http://jtr.zhongyouzk.top

Py:   s.splitlines()
来源：http://jys.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lhs.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://trm.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://zii.tarul.cn

Java: s.lines().toList()
来源：http://ahh.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://awq.xuetiantiany.cn

Ruby: s.lines
来源：http://lgh.yongpay.top

C#:   s.Split('\n')
来源：http://gez.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://pso.jinqigufen.top

Py:   if not s:
来源：http://hwn.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uvj.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ulh.bjfxy.top

TS:   if (s === "") {}
来源：http://quf.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://djg.chenlongwang.top

Go:   if s == "" {}
来源：http://bcq.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://xpc.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lku.wangshuangyany.cn

[E21] 超长截断加省略号
来源：http://dbh.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xnn.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wga.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tep.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ndz.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zex.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://xej.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ykf.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zfy.yj202588.top

[E22] 字节长度与字符长度
来源：http://xnm.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pte.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fdw.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cbn.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nvf.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vcz.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yso.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://dfe.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://noy.aizwys.cn

================================================================================
来源：http://ipe.52xcode.cn

F. 文件与目录
来源：http://uvk.c1oappe.top

================================================================================
来源：http://xhy.daxiang520.top

[F01] 读取整个文件
来源：http://sqw.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ije.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://snw.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://civ.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tta.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://txb.snrcjt.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fvx.jianghu66.top

Ruby: File.read("a.txt")
来源：http://bip.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://cyr.hnqzz.top

[F02] 逐行读取文件
来源：http://txd.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ljb.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ygw.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hpy.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zvf.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xmw.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kxx.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nez.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lhc.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://iyk.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cnd.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cju.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ais.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kkt.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://glh.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fnu.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://mda.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rbu.tarul.cn

[F04] 追加写入文件
来源：http://htt.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gmz.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ulm.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ipe.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dse.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cqb.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yuo.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tuq.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://slc.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://mjh.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ily.tarul.cn

PHP:  file_exists("a.txt");
来源：http://jzh.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://pcb.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://xmp.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://std.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aen.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://igg.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://fuv.uphjek.com

[F06] 删除文件
来源：http://dcz.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://xzw.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://yre.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://afs.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dco.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tey.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://gxh.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://xqy.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://gea.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://pmk.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tle.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cud.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uxc.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jct.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qgq.tian-w.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fxa.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gns.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://teu.cqqwz.cn

[F08] 遍历目录
来源：http://oha.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ftg.aizwys.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aha.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://qwn.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://yee.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uuw.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zsp.xuanzx.com

Ruby: Dir.children("dir")
来源：http://vkr.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://heh.zdbjq.cn

[F09] 获取文件大小
来源：http://fvl.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://zgs.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://iwi.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://ret.hnqzz.top

TS:   fs.statSync("a.txt").size
来源：http://zma.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://soj.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jsm.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://djm.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://mil.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://vto.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iwq.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://afw.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lod.tanke756.top

TS:   path.extname("a.txt")
来源：http://fgd.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fix.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://olh.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hhq.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vwa.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://fpv.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uac.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mvs.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ody.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pab.epnwcf.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fqr.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jih.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hgq.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wbp.epnwcf.com

[F12] CSV 读写
来源：http://imm.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gav.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://euc.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mnz.fzhhl.top

TS:   // 同上
来源：http://qfw.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vem.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hwl.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://upj.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://eim.jqgufenzy.top

================================================================================
来源：http://uuq.c1oappe.top

G. 面向对象
来源：http://eul.cucudq.cn

================================================================================
来源：http://gvr.wangshuangyany.cn

[G01] 定义类
来源：http://eyg.yj20258.top


<!-- 参考信息 -->