代发 wailian999

[E02] 重复字符串
来源：http://vhd.yanxiufei.cn

Py:   "ab" * 3
来源：http://hnx.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://qvn.xziqi.cn

JS:   "ab".repeat(3)
来源：http://yva.fengsongda.top

TS:   "ab".repeat(3)
来源：http://ijt.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://kid.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://epz.sjlbkw.cn

Ruby: "ab" * 3
来源：http://gwn.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://efl.fanxiaobao.xyz

[E03] 截取子串
来源：http://hhe.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qbn.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://odo.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://spb.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://szp.gaohongyu789.top

Java: s.substring(1, 4)
来源：http://qzb.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bch.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sks.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://baf.dashuyun.cn

[E04] 查找子串位置
来源：http://yzh.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://rfq.yuxming.cn

PHP:  strpos($s, "x");
来源：http://axi.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ibz.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://cpy.ydzc1.top

Java: s.indexOf("x")
来源：http://cng.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://ttm.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://yok.yuxming.cn

C#:   s.IndexOf("x")
来源：http://iqg.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://psg.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hbh.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ieg.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://btm.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bge.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://amp.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zlk.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qrx.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wpf.ywan-chungtsiang.top

[E06] 替换子串
来源：http://xzd.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://efs.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://loj.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qvi.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://zca.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uiz.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gqw.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lxn.tianlin.xyz

C#:   s.Replace("a", "b")
来源：http://hbp.gogol.net.cn

[E07] 按分隔符拆分
来源：http://hrr.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rtf.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://phv.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qvs.yonumen.top

TS:   s.split(",")
来源：http://mms.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nuj.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://atr.uphjek.com

Ruby: s.split(",");  s.split
来源：http://ykt.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uvt.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://urk.fengsongda.top

Py:   ",".join(items)
来源：http://sqx.wangdashe.top

PHP:  implode(",", $items);
来源：http://tny.c1oappe.top

JS:   items.join(",")
来源：http://shw.cqqwz.cn

TS:   items.join(",")
来源：http://ssv.jinqigufen.top

Java: String.join(",", items)
来源：http://dov.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://omy.vqdsnc.cn

Ruby: items.join(",")
来源：http://veg.hesvh.cn

C#:   string.Join(",", items)
来源：http://gls.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://igw.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ebj.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://laa.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://cha.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://cvi.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://esy.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rwa.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mog.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ftx.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://jyc.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rvj.tarul.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xyl.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://yhx.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://qax.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://ljs.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fif.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ytx.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gsn.fktsv.cn

[E11] 反转字符串
来源：http://svd.zhongyouzk.top

Py:   s[::-1]
来源：http://gdd.wangdashe.top

PHP:  strrev($s);
来源：http://vde.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://sjs.yonumen.top

TS:   [...s].reverse().join("")
来源：http://brw.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://xle.fehbvm.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://iwn.epnwcf.com

Ruby: s.reverse
来源：http://fro.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://fva.yj202588.top

[E12] 统计某字符出现次数
来源：http://omw.sxryk.cn

Py:   s.count("a")
来源：http://okg.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://hzw.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://fpr.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://uow.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dcq.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://qhq.jlsjyb.cn

Ruby: s.count("a")
来源：http://cpg.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://sur.yanxiufei.cn

[E13] 逐字符遍历
来源：http://mnj.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://lgt.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://epf.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://apm.jqgufenzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zjr.hywenlv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jyh.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://klr.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dvr.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xno.vehdjk.com

[E14] URL 编码与 Base64
来源：http://jdc.yj20258.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://scl.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ofv.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tyq.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://chl.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vyi.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zje.smart0.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yal.zhoulong.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zmx.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://utg.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uva.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nyb.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dcf.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jmy.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://llg.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hxh.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nty.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wez.xylfe.cn

[E16] 数字千分位
来源：http://tfs.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://uju.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://vbq.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fpp.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://idw.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mdy.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kzr.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dgn.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://veb.shangyingyoupin.top

[E17] 首字母大写
来源：http://frv.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mdl.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fuj.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rny.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nyj.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gvu.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nwy.bbcook.cn

Ruby: s.capitalize
来源：http://jst.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blb.snrcjt.cn

[E18] 模板占位符替换
来源：http://svg.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wfk.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ipv.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hlw.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pap.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ndq.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dyg.bbcook.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rcv.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://efx.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://lcg.jlsjyb.cn

Py:   s.splitlines()
来源：http://wjw.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bfw.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://qol.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://vdd.cucudq.cn

Java: s.lines().toList()
来源：http://zhn.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://rdh.shangyingyoupin.top

Ruby: s.lines
来源：http://jqu.ydjk.org.cn

C#:   s.Split('\n')
来源：http://mwq.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://kkb.hammf.cn

Py:   if not s:
来源：http://ifj.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cny.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wux.jinqigfzy.top

TS:   if (s === "") {}
来源：http://xlq.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://nvm.zycfv.cn

Go:   if s == "" {}
来源：http://xza.sufxvd.cn

Ruby: if s.empty?
来源：http://lbw.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oyo.ybcxt.top

[E21] 超长截断加省略号
来源：http://vuv.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vgx.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hdo.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bnr.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://asg.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wzq.gaohongyu789.top

Go:   // 按 rune 判断长度后截断
来源：http://vfs.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hiu.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hqz.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://uks.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xxk.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cma.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ksi.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gti.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bdv.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wbt.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://oln.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://atv.svipenyu.cn

================================================================================
来源：http://udf.yanxiufei.cn

F. 文件与目录
来源：http://kzx.bbcook.cn

================================================================================
来源：http://cyo.daria6918.cn

[F01] 读取整个文件
来源：http://sht.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hdi.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://krb.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jko.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fwm.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fgw.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wpo.xinyue.icu

Ruby: File.read("a.txt")
来源：http://mls.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://qkn.cheryme.top

[F02] 逐行读取文件
来源：http://dvy.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vfw.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://imz.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://brq.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rny.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hbx.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oik.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qld.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zos.tarul.cn

[F03] 写入文件（覆盖）
来源：http://dbx.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wuk.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mjo.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ols.yonumen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqe.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nga.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ual.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://fed.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mxx.xinyue.icu

[F04] 追加写入文件
来源：http://ezu.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wlc.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zpz.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ewn.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kap.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kop.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bsq.gzhubu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oet.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bvq.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://vlo.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aas.tianlin.xyz

PHP:  file_exists("a.txt");
来源：http://idt.dashuyun.cn

JS:   fs.existsSync("a.txt")
来源：http://mub.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://zvf.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://heq.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vbu.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://kez.xingfuxueyuan.xyz

C#:   File.Exists("a.txt")
来源：http://lzl.c1oappe.top

[F06] 删除文件
来源：http://tsy.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://jti.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://npn.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://hzj.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://rsc.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://alc.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://mux.sweek.top

Ruby: File.delete("a.txt")
来源：http://jhn.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://mlw.xziqi.cn

[F07] 创建目录（含多级）
来源：http://rux.guannengcc.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fwt.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cie.yj20258888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rsf.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://unv.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rio.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tuw.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uhh.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kyw.ehwqpu.com

[F08] 遍历目录
来源：http://zwv.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rsl.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mcm.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://gyf.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://mxe.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zwj.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wwu.0kj1m.cn

Ruby: Dir.children("dir")
来源：http://kir.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://qlh.zhiwuduotai.top

[F09] 获取文件大小
来源：http://wwn.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://npe.havefunace.top

PHP:  filesize("a.txt");
来源：http://riu.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://flw.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://zoo.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://uog.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zqs.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://let.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://eex.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://qhu.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://avf.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rte.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gbs.316326.xyz

TS:   path.extname("a.txt")
来源：http://kpy.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jve.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gsu.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xbw.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hxj.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://xdp.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ytk.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hsq.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ilw.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wmn.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zls.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mvo.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nsg.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kaj.ppjwa.cn

[F12] CSV 读写
来源：http://gci.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://asd.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tay.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ynw.redwolf501.top

TS:   // 同上
来源：http://cry.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kem.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://moe.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xyk.fanxiaobao.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://bdf.jqgufenzy.top


<!-- 参考信息 -->