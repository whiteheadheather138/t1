代发 wailian999

[E02] 重复字符串
来源：http://afj.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://wsv.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://xve.gzhubu.top

JS:   "ab".repeat(3)
来源：http://jtr.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://rlw.jyoumei.cn

Java: "ab".repeat(3)
来源：http://jso.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://tyd.hywenlv.cn

Ruby: "ab" * 3
来源：http://byk.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yki.xylfe.cn

[E03] 截取子串
来源：http://wzn.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lbj.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cfp.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ftl.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://wuq.guannengcc.top

Java: s.substring(1, 4)
来源：http://uqk.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pqz.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://khz.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://luj.gogol.net.cn

[E04] 查找子串位置
来源：http://gjk.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://pzh.uphjek.com

PHP:  strpos($s, "x");
来源：http://ebi.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ggb.xylfe.cn

TS:   s.indexOf("x")
来源：http://ron.yueranfly.top

Java: s.indexOf("x")
来源：http://ibx.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://zry.52xcode.cn

Ruby: s.index("x")
来源：http://aod.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://zmq.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zvh.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cok.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iev.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hpb.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ewa.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tnp.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xfw.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ewg.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://szx.uphjek.com

[E06] 替换子串
来源：http://emu.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qqg.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://eaa.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dst.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://wck.hesvh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oyb.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fce.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fmk.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://vvm.tarul.cn

[E07] 按分隔符拆分
来源：http://hob.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eqr.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tar.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ebu.smart0.xyz

TS:   s.split(",")
来源：http://qcc.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://eku.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rto.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://lok.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nvs.nwbrower.top

[E08] 数组按分隔符合并
来源：http://jrl.tian-w.cn

Py:   ",".join(items)
来源：http://yaw.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://tmq.quarkkingdee.top

JS:   items.join(",")
来源：http://hlp.chenlongwang.top

TS:   items.join(",")
来源：http://vto.sweek.top

Java: String.join(",", items)
来源：http://mjk.hcnkem.com

Go:   strings.Join(items, ",")
来源：http://rge.hongshengwenyu.top

Ruby: items.join(",")
来源：http://gih.guowangkeji.top

C#:   string.Join(",", items)
来源：http://qrg.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://vxu.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hqg.iojbl.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://els.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://uhu.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://tmg.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://wuj.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lpu.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bcd.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vsf.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://vta.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://meu.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qbr.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://qrj.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://wuq.gzhubu.top

Java: String.format("%03d", 7)
来源：http://cde.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pqa.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fzh.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lno.zdbjq.cn

[E11] 反转字符串
来源：http://mat.dianchejie.cn

Py:   s[::-1]
来源：http://wes.hnqzz.top

PHP:  strrev($s);
来源：http://wdi.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://rmc.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://fux.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://afx.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wgm.dashuyun.cn

Ruby: s.reverse
来源：http://tvj.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kgm.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://gtg.jianghu66.top

Py:   s.count("a")
来源：http://mol.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://kqf.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://dva.xylfe.cn

TS:   s.split("a").length - 1
来源：http://ezm.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aph.ivvv.top

Go:   strings.Count(s, "a")
来源：http://vdi.sweek.top

Ruby: s.count("a")
来源：http://csp.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://amn.52xcode.cn

[E13] 逐字符遍历
来源：http://vgi.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://vty.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bcp.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kln.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gnk.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iwv.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://res.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://awt.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tyu.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://zxm.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wwg.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jsc.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ohe.xinyue.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rqk.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qfl.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sjh.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://phj.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nan.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://mvq.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ajw.52xcode.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fit.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://frt.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lvg.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://enc.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ztg.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pty.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qdr.fanxiaobao.xyz

[E16] 数字千分位
来源：http://wbt.cucudq.cn

Py:   f"{1234567:,}"
来源：http://tgs.yongpay.top

PHP:  number_format(1234567);
来源：http://dzp.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yvj.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hfy.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ekv.nanxinkj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cyr.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zeh.sweek.top

C#:   1234567.ToString("N0")
来源：http://dgv.redwolf501.top

[E17] 首字母大写
来源：http://rph.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hco.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ccd.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cbd.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hep.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cxn.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jte.sufxvd.cn

Ruby: s.capitalize
来源：http://tgo.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mcd.yuxming.cn

[E18] 模板占位符替换
来源：http://wmi.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wne.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bks.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zua.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sgo.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lyv.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lmj.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sbo.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pfq.havefunace.top

[E19] 多行文本按行拆分
来源：http://ogb.chenzaomai.com

Py:   s.splitlines()
来源：http://afr.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kvl.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://dyj.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://ehe.xziqi.cn

Java: s.lines().toList()
来源：http://jit.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://hls.aizwys.cn

Ruby: s.lines
来源：http://khq.yangfankeji.com

C#:   s.Split('\n')
来源：http://lxk.shanyushiyangkeji.top

[E20] 判断字符串是否为空
来源：http://kni.vqdsnc.cn

Py:   if not s:
来源：http://swt.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vec.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hzr.iojbl.cn

TS:   if (s === "") {}
来源：http://pky.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://yoj.zhiwuduotai.top

Go:   if s == "" {}
来源：http://hyv.aizwys.cn

Ruby: if s.empty?
来源：http://uic.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gds.ivvv.top

[E21] 超长截断加省略号
来源：http://oxm.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uar.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mfp.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yhw.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tyk.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://csr.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://kth.guannengcc.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lwu.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ozz.daxiang520.top

[E22] 字节长度与字符长度
来源：http://jui.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bur.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yiu.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rul.cqqwz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hpx.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://diz.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sez.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://emk.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mph.jinqigufen.top

================================================================================
来源：http://vln.uphjek.com

F. 文件与目录
来源：http://dhw.sxryk.cn

================================================================================
来源：http://zgc.kuanghao11.cn

[F01] 读取整个文件
来源：http://bww.cdnleiting.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aak.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://msa.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://egy.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zoe.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ons.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://awy.yanxiufei.cn

Ruby: File.read("a.txt")
来源：http://rvc.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://xjv.jianghu66.top

[F02] 逐行读取文件
来源：http://hsp.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ulf.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://heg.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://faq.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iyu.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://huh.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nok.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mar.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://flp.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://fts.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hca.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wzi.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jom.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rnf.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nnb.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nmz.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://hic.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sra.gogol.net.cn

[F04] 追加写入文件
来源：http://vpq.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yus.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zuc.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qoo.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ixd.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uet.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ihl.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nhw.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sgx.chenzaomai.com

[F05] 判断文件或目录是否存在
来源：http://mgj.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ceb.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://tsr.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://fog.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://hki.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://qug.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vut.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://hqo.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://aws.cheryme.top

[F06] 删除文件
来源：http://cuc.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://xjh.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://dwh.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://uzj.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://klz.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uph.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://kyv.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://mbu.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://epc.ydzc1.top

[F07] 创建目录（含多级）
来源：http://skk.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lrs.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vmt.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zfb.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uzq.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lzf.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zkk.ehwqpu.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://noc.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gwk.hysaishi.cn

[F08] 遍历目录
来源：http://aby.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://foi.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wpr.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://bgy.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://nir.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bft.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://gfe.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://wqf.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://ptu.hnqzz.top

[F09] 获取文件大小
来源：http://kag.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://tro.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://ufh.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://mde.svipenyu.cn

TS:   fs.statSync("a.txt").size
来源：http://krq.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://usn.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wgz.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://cmm.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://xyy.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://xpm.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jil.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://atf.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gic.fzhhl.top

TS:   path.extname("a.txt")
来源：http://nif.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nqu.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pus.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ign.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://coh.redwolf501.top

[F11] 复制与移动文件
来源：http://gja.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gjg.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pqh.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://loj.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfi.jiagoushi.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eph.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aub.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ouo.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tes.shuidangran.top

[F12] CSV 读写
来源：http://dta.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rgj.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fds.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rjl.hywenlv.cn

TS:   // 同上
来源：http://dpx.jiagoushi.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hge.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gtf.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jqh.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xrh.zhiwuduotai.top


<!-- 参考信息 -->