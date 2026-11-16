代发 wailian999

TS:   "ab".repeat(3)
来源：http://iha.daxiang520.top

Java: "ab".repeat(3)
来源：http://tfi.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://viu.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://qym.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wkd.chenjidiqi.icu

[E03] 截取子串
来源：http://iza.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://doo.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rxu.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://luw.xylfe.cn

TS:   s.slice(1, 4)
来源：http://nxm.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://gjc.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ypp.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://van.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://ekr.hnqzz.top

[E04] 查找子串位置
来源：http://vxm.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://pqo.52xcode.cn

PHP:  strpos($s, "x");
来源：http://dtl.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cgx.nwbrower.top

TS:   s.indexOf("x")
来源：http://cqe.yvedp.cn

Java: s.indexOf("x")
来源：http://trt.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://kvf.tanke756.top

Ruby: s.index("x")
来源：http://jgf.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://xzy.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nng.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://krk.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lif.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zrk.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://uds.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lnn.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://udk.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rfr.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xxk.yongpay.top

[E06] 替换子串
来源：http://xyr.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://min.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://dzj.yfazqb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kfm.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://yve.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cqi.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yma.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cfw.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://wzn.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://cbc.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://okq.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pmu.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pwg.sweek.top

TS:   s.split(",")
来源：http://kys.jyoumei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eqg.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iod.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://npl.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zsk.cheryme.top

[E08] 数组按分隔符合并
来源：http://psl.ydjk.org.cn

Py:   ",".join(items)
来源：http://xju.nwbrower.top

PHP:  implode(",", $items);
来源：http://gis.cucudq.cn

JS:   items.join(",")
来源：http://pni.mhx1999.top

TS:   items.join(",")
来源：http://pzu.yanxiufei.cn

Java: String.join(",", items)
来源：http://amn.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://fac.zdbjq.cn

Ruby: items.join(",")
来源：http://mou.ivvv.top

C#:   string.Join(",", items)
来源：http://ise.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://oni.sjlbkw.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ymk.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://adu.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://pln.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://fqt.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://puq.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fcm.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://ouh.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gop.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://zzj.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ewk.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ank.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://eeu.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://rox.yfazqb.com

Java: String.format("%03d", 7)
来源：http://dck.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pff.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://inc.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ffy.sxryk.cn

[E11] 反转字符串
来源：http://rko.vehdjk.com

Py:   s[::-1]
来源：http://vvd.yj20258888.top

PHP:  strrev($s);
来源：http://ejm.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://pqw.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://fhw.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://khl.ybcxt.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kmy.andypj.xyz

Ruby: s.reverse
来源：http://cdo.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://uer.pycfn.com

[E12] 统计某字符出现次数
来源：http://stt.316326.xyz

Py:   s.count("a")
来源：http://aln.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://jhg.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://zqs.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://tfd.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://juu.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://gmv.yongpay.top

Ruby: s.count("a")
来源：http://lcv.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://cqt.gaohongyu789.top

[E13] 逐字符遍历
来源：http://tcv.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://eqc.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bce.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://zhe.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wwi.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://onk.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mrm.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kgh.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://luc.yangfankeji.com

[E14] URL 编码与 Base64
来源：http://fou.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uwx.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://acv.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ayi.kuanghao11.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jrb.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mmq.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iml.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kyh.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zyg.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://nek.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ctj.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jux.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jou.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xlz.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xdm.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vgv.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ztg.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bda.jinghuilouyu.cn

[E16] 数字千分位
来源：http://wwe.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://jyh.xziqi.cn

PHP:  number_format(1234567);
来源：http://wpw.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rjj.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hbz.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://quw.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ilz.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jqj.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://yao.yj20258.top

[E17] 首字母大写
来源：http://uix.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tgl.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://huq.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://siw.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pbt.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://udr.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oxf.fengsongda.top

Ruby: s.capitalize
来源：http://wvy.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gub.fehbvm.com

[E18] 模板占位符替换
来源：http://myd.daria6918.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bgs.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tmu.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://nif.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://hhi.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iay.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ipe.jinyuanbaomall.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vsq.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://laq.fktsv.cn

[E19] 多行文本按行拆分
来源：http://fdh.chenjidiqi.icu

Py:   s.splitlines()
来源：http://kys.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cuw.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://pho.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://vos.havefunace.top

Java: s.lines().toList()
来源：http://dzl.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://qvb.yfazqb.com

Ruby: s.lines
来源：http://pvu.jiagoushi.top

C#:   s.Split('\n')
来源：http://ogm.tian-w.cn

[E20] 判断字符串是否为空
来源：http://mra.yanxiufei.cn

Py:   if not s:
来源：http://onp.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vix.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qsn.quarkkingdee.top

TS:   if (s === "") {}
来源：http://usk.shzxlz.cn

Java: if (s.isEmpty()) {}
来源：http://ayq.nwbrower.top

Go:   if s == "" {}
来源：http://anj.ydzc1.top

Ruby: if s.empty?
来源：http://frl.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://otl.hcnkem.com

[E21] 超长截断加省略号
来源：http://gkl.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ivp.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tqj.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ecj.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xpb.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kge.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://eqt.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ewh.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hfn.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://xct.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://osg.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qrj.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rxr.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dny.jinqigfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wfh.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jca.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://zsn.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cvx.zhengqikj.top

================================================================================
来源：http://vjo.fanxiaobao.xyz

F. 文件与目录
来源：http://nsd.redwolf501.top

================================================================================
来源：http://pjz.zhiwuduotai.top

[F01] 读取整个文件
来源：http://xts.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iiu.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://dar.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bvy.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xlw.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kpd.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wlg.epnwcf.com

Ruby: File.read("a.txt")
来源：http://fri.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://mpi.pycfn.com

[F02] 逐行读取文件
来源：http://uuv.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jzk.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jon.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mix.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rlq.0kj1m.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ajy.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ias.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zht.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bls.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://iur.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://myf.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xoa.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wkf.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wzr.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lzf.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wna.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://obm.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kdn.fzhhl.top

[F04] 追加写入文件
来源：http://vhp.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pcd.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kbb.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ezk.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eiu.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nwq.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://byw.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://trf.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zai.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://rgt.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://anl.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://tjd.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://clr.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://jgl.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vhc.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://evk.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://vte.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://ngc.aibaodan.cn

[F06] 删除文件
来源：http://nbl.fehbvm.com

Py:   os.remove("a.txt")
来源：http://mrc.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://yxg.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://irk.gaohongyu789.top

TS:   fs.unlinkSync("a.txt")
来源：http://aty.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ood.uphjek.com

Go:   os.Remove("a.txt")
来源：http://zis.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://wxz.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://kfe.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://prr.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ltr.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fqt.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kyn.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ojv.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bxm.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fme.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sos.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ytg.nanxuanxn.top

[F08] 遍历目录
来源：http://jct.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://lax.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qzm.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://luj.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://epu.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gup.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://kle.nwbrower.top

Ruby: Dir.children("dir")
来源：http://qdm.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://dth.svipenyu.cn

[F09] 获取文件大小
来源：http://izc.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://fjw.hesvh.cn

PHP:  filesize("a.txt");
来源：http://ovl.yuxming.cn

JS:   fs.statSync("a.txt").size
来源：http://fqh.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://xtp.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://iwb.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kxl.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://ivp.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://gva.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://wuo.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wpi.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vng.ppjwa.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rnh.ybcxt.top

TS:   path.extname("a.txt")
来源：http://qsr.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://stj.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pyh.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eva.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://udm.iojbl.cn

[F11] 复制与移动文件
来源：http://fig.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zny.sjlbkw.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hyf.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mkf.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vpw.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ewi.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yiw.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://duj.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://chq.feifeiyinyue.top

[F12] CSV 读写
来源：http://drb.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://udc.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xav.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sge.pycfn.com

TS:   // 同上
来源：http://swd.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ngi.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gyq.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://boa.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://njh.wangshuangyany.cn

================================================================================
来源：http://ahp.gaohongyu789.top

G. 面向对象
来源：http://aea.zdqjudy.top

================================================================================
来源：http://tva.jinqigufen.top

[G01] 定义类
来源：http://ujg.jiagoushi.top


<!-- 参考信息 -->