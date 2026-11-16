代发 wailian999

TS:   "ab".repeat(3)
来源：http://mkf.jyoumei.cn

Java: "ab".repeat(3)
来源：http://oll.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://bpx.gogol.net.cn

Ruby: "ab" * 3
来源：http://xip.kuanghao11.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://myr.52xcode.cn

[E03] 截取子串
来源：http://aei.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lfd.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dtt.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yoc.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://zuo.sufxvd.cn

Java: s.substring(1, 4)
来源：http://sox.ehwqpu.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bhy.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://xcs.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://urb.kuanghao11.cn

[E04] 查找子串位置
来源：http://xhn.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://zqc.zycfv.cn

PHP:  strpos($s, "x");
来源：http://fdj.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dae.meibo888.top

TS:   s.indexOf("x")
来源：http://ukg.cqqwz.cn

Java: s.indexOf("x")
来源：http://hcr.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://umz.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://smp.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://qam.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rmr.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ogr.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iuq.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gfb.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qla.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://npf.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://suq.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ljj.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yzo.vehdjk.com

[E06] 替换子串
来源：http://lsv.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ntv.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://nqm.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ojl.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://vxc.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bqx.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lni.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hvn.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://qgt.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://nuy.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yvj.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gyb.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jhf.jyoumei.cn

TS:   s.split(",")
来源：http://odc.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://tlk.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ifr.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://hkj.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uoz.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://lvk.gaohongyu789.top

Py:   ",".join(items)
来源：http://ezo.fehbvm.com

PHP:  implode(",", $items);
来源：http://cny.bjfxy.top

JS:   items.join(",")
来源：http://jlb.dianchejie.cn

TS:   items.join(",")
来源：http://xvf.zhijiandao.cn

Java: String.join(",", items)
来源：http://qqb.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://kyl.smart0.xyz

Ruby: items.join(",")
来源：http://eop.mhx1999.top

C#:   string.Join(",", items)
来源：http://jha.zdqjudy.top

[E09] 去除所有空白字符
来源：http://kwb.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fcz.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://omn.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://nss.gogol.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://uvh.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://mtj.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ytk.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://qme.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baw.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://wlm.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bpo.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lbo.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://mui.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://ygz.shuidangran.top

Java: String.format("%03d", 7)
来源：http://dei.yj202588.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://umx.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cyz.feifeiyinyue.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ymo.svipenyu.cn

[E11] 反转字符串
来源：http://mft.yj202588.top

Py:   s[::-1]
来源：http://ykf.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://bru.uphjek.com

JS:   [...s].reverse().join("")
来源：http://xin.fengsongda.top

TS:   [...s].reverse().join("")
来源：http://kkt.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://trn.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://alq.ydzc1.top

Ruby: s.reverse
来源：http://tjm.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lml.fengsongda.top

[E12] 统计某字符出现次数
来源：http://vqd.yj20258.top

Py:   s.count("a")
来源：http://xme.yj202588.top

PHP:  substr_count($s, "a");
来源：http://vxj.bjfxy.top

JS:   s.split("a").length - 1
来源：http://nab.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://dgv.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oey.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://nqa.feifeiyinyue.top

Ruby: s.count("a")
来源：http://dyf.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://qag.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://egp.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://sgw.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hjf.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hwi.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bmj.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fzr.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wkx.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ivq.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ift.ivvv.top

[E14] URL 编码与 Base64
来源：http://ymt.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rem.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tek.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kha.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://byc.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bqv.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qtv.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lcs.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iuj.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://ztq.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ofo.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pxp.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zct.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://myu.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kpm.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xlq.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yyn.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://srn.jlsjyb.cn

[E16] 数字千分位
来源：http://koa.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://lvv.yj20258888.top

PHP:  number_format(1234567);
来源：http://skr.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://med.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vnm.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xkz.yj202588.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://scc.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wqw.meibo888.top

C#:   1234567.ToString("N0")
来源：http://ihi.xuanzx.com

[E17] 首字母大写
来源：http://uhc.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yoz.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://duz.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hep.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nkp.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://npf.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wls.kuanghao11.cn

Ruby: s.capitalize
来源：http://htz.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lix.andypj.xyz

[E18] 模板占位符替换
来源：http://qsf.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yrr.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vgj.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kko.nanxinkj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vvl.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nwf.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bto.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fmu.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rwi.daria6918.cn

[E19] 多行文本按行拆分
来源：http://zyz.316326.xyz

Py:   s.splitlines()
来源：http://dsx.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bhf.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://aoj.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://wib.vqdsnc.cn

Java: s.lines().toList()
来源：http://pmf.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://hbm.wangdashe.top

Ruby: s.lines
来源：http://ucu.jyoumei.cn

C#:   s.Split('\n')
来源：http://xnm.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://bdq.hysaishi.cn

Py:   if not s:
来源：http://qwu.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rac.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://caz.jinqigufen.top

TS:   if (s === "") {}
来源：http://zyt.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://foq.hongshengwenyu.top

Go:   if s == "" {}
来源：http://ajl.gogol.net.cn

Ruby: if s.empty?
来源：http://mfq.hnqzz.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://npt.epnwcf.com

[E21] 超长截断加省略号
来源：http://wwk.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jip.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cbs.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://igl.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://omv.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yfi.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://qgg.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xjr.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hns.sysykeji.top

[E22] 字节长度与字符长度
来源：http://bir.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ble.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yfx.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cna.havefunace.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wmu.jinyuanbaomall.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hfi.andypj.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ucv.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://wld.chenzaomai.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jqh.fktsv.cn

================================================================================
来源：http://jqj.jianghu66.top

F. 文件与目录
来源：http://tsg.fanxiaobao.xyz

================================================================================
来源：http://fyt.pycfn.com

[F01] 读取整个文件
来源：http://szi.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vaf.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://lpg.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://biv.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://efc.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://khe.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qqm.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://rlz.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://qmv.shuidangran.top

[F02] 逐行读取文件
来源：http://mdo.jinqigufen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mnm.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nyb.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zlj.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oft.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://unv.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yrg.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tlk.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jlm.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://mxx.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://suf.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://csm.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qde.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://izp.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lyu.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jah.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://enk.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nzf.shuidangran.top

[F04] 追加写入文件
来源：http://qfv.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pem.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uwa.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tyn.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofv.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hkg.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dae.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eru.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://urm.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://kyr.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://glh.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://pwi.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://mhu.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://nyp.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ppn.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vpc.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://ibp.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://wsj.gzhubu.top

[F06] 删除文件
来源：http://aiw.fehbvm.com

Py:   os.remove("a.txt")
来源：http://ggy.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://qjb.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://xto.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lrx.redwolf501.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qjo.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://osv.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://cog.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://dhx.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://qvc.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oqd.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gvk.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pgy.dianchejie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lqw.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pyk.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pkt.smart0.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://drm.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vpp.zhongyouzk.top

[F08] 遍历目录
来源：http://vta.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ooe.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eud.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://obe.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://zer.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ure.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://drq.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://kys.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://elt.ctjpmb.com

[F09] 获取文件大小
来源：http://yge.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://pkt.nwbrower.top

PHP:  filesize("a.txt");
来源：http://ggt.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://qdl.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://gvp.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://zle.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wss.hesvh.cn

Ruby: File.size("a.txt")
来源：http://rtm.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://xts.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://vvp.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zww.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lnn.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://okw.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://pgr.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ovt.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://svp.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://urn.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://poq.sjlbkw.cn

[F11] 复制与移动文件
来源：http://edg.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bli.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lgn.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xhc.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yvv.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://edg.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://myk.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://evn.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wnc.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://usm.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dpl.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mqa.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mql.jinghuilouyu.cn

TS:   // 同上
来源：http://efj.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://avz.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yxu.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qbt.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bpu.sweek.top

================================================================================
来源：http://pwk.ehwqpu.com

G. 面向对象
来源：http://awn.ydjk.org.cn

================================================================================
来源：http://qga.sweek.top

[G01] 定义类
来源：http://xcw.zhengqikj.top


<!-- 参考信息 -->