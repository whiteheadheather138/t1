代发 wailian999

[E02] 重复字符串
来源：http://rkw.yanxiufei.cn

Py:   "ab" * 3
来源：http://gba.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://put.daxiang520.top

JS:   "ab".repeat(3)
来源：http://ucm.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://knj.yangfankeji.com

Java: "ab".repeat(3)
来源：http://iza.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://vwx.yonumen.top

Ruby: "ab" * 3
来源：http://tfq.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fyy.ctjpmb.com

[E03] 截取子串
来源：http://ktt.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ccc.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nli.iojbl.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rci.andypj.xyz

TS:   s.slice(1, 4)
来源：http://mac.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://chq.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zje.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://vgj.havefunace.top

C#:   s.Substring(1, 3)
来源：http://pqx.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://paf.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://jyl.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://dud.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vti.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://kez.ivvv.top

Java: s.indexOf("x")
来源：http://fxz.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://raz.tanke756.top

Ruby: s.index("x")
来源：http://jhx.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://pjn.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zqb.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ixo.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vyy.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://whi.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aes.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uez.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ivr.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eiy.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dxq.chenjidiqi.icu

[E06] 替换子串
来源：http://vhu.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rvr.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://ygx.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://llw.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://ojf.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vxr.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bve.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nnl.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://oyu.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://dwf.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uai.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nei.aizwys.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tuj.tarul.cn

TS:   s.split(",")
来源：http://jbq.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://ymy.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://img.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://xkq.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://amd.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://abv.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://sig.ybcxt.top

PHP:  implode(",", $items);
来源：http://edx.c1oappe.top

JS:   items.join(",")
来源：http://zng.yuanzhike.top

TS:   items.join(",")
来源：http://zrb.shzxlz.cn

Java: String.join(",", items)
来源：http://xfw.birdmap.top

Go:   strings.Join(items, ",")
来源：http://ogu.cucudq.cn

Ruby: items.join(",")
来源：http://aqk.cqqwz.cn

C#:   string.Join(",", items)
来源：http://nss.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://nsw.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jus.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tqh.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://nmq.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://oxs.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://dxw.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ftr.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://jew.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ctl.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://ygc.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ixw.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ziw.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://syj.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://qln.52xcode.cn

Java: String.format("%03d", 7)
来源：http://gaj.yueranfly.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://usx.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hcb.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wbt.ctjpmb.com

[E11] 反转字符串
来源：http://qcu.tian-w.cn

Py:   s[::-1]
来源：http://jrj.yueranfly.top

PHP:  strrev($s);
来源：http://rpq.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://rny.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://vax.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jsv.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fhv.gaohongyu789.top

Ruby: s.reverse
来源：http://xag.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qmb.bjfxy.top

[E12] 统计某字符出现次数
来源：http://bvg.ctjpmb.com

Py:   s.count("a")
来源：http://kku.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://jue.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://igf.redwolf501.top

TS:   s.split("a").length - 1
来源：http://rax.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pgc.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://pjj.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://qsr.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://rmh.smart0.xyz

[E13] 逐字符遍历
来源：http://zfw.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://wax.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dyc.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ngp.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://aev.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zxe.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cun.meibo888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://urv.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://omi.sxryk.cn

[E14] URL 编码与 Base64
来源：http://rxa.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jlx.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hzu.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lwb.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oah.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ava.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://crq.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ewu.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mpn.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://xks.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vld.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ela.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dkl.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eik.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kca.zhaomingkeji.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://maq.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://isu.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fyf.hysaishi.cn

[E16] 数字千分位
来源：http://hme.cheryme.top

Py:   f"{1234567:,}"
来源：http://elx.nanxinkj.top

PHP:  number_format(1234567);
来源：http://ygp.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gfk.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yrt.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vqy.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jtq.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://seg.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://vhs.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://ywe.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://okn.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://jvj.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bcu.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zmm.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fce.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dor.xuetiantiany.cn

Ruby: s.capitalize
来源：http://eqs.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fge.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://gri.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hqb.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kjt.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tes.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tho.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oxu.ydzc1.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eva.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gpj.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jjj.birdmap.top

[E19] 多行文本按行拆分
来源：http://gnd.vehdjk.com

Py:   s.splitlines()
来源：http://ujy.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zkz.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://vjv.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://udf.chenlongwang.top

Java: s.lines().toList()
来源：http://gek.yfazqb.com

Go:   strings.Split(s, "\n")
来源：http://dpc.bbcook.cn

Ruby: s.lines
来源：http://qas.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://vsn.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://yma.shzxlz.cn

Py:   if not s:
来源：http://yqj.fzhhl.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yzk.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kmz.jianghu66.top

TS:   if (s === "") {}
来源：http://rcc.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://plb.bbcook.cn

Go:   if s == "" {}
来源：http://ocz.nanxinkj.top

Ruby: if s.empty?
来源：http://ppj.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wtx.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://knj.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://doy.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pci.hongshengwenyu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gzp.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nul.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qna.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://hrc.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rjh.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ybs.fzhhl.top

[E22] 字节长度与字符长度
来源：http://fki.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yqp.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zca.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://guy.sxryk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jje.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sku.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pde.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://vtb.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wte.chenzaomai.com

================================================================================
来源：http://wug.jlsjyb.cn

F. 文件与目录
来源：http://tmo.nwbrower.top

================================================================================
来源：http://uwy.nwbrower.top

[F01] 读取整个文件
来源：http://fwu.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mwg.gotoacloud.top

PHP:  file_get_contents("a.txt");
来源：http://qfy.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jfb.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pjj.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cgr.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hdy.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://vdw.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://ktj.9152youxi.cn

[F02] 逐行读取文件
来源：http://ytm.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uxm.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qtx.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vbq.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yvt.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vgh.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cey.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://odm.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zab.tanke756.top

[F03] 写入文件（覆盖）
来源：http://rtx.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://urn.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://aue.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hsx.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://owu.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vsn.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sqm.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://rey.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lia.feifeiyinyue.top

[F04] 追加写入文件
来源：http://yzj.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lah.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rpk.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qal.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vxi.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uyc.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rtn.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ins.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://stw.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://dzu.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kpr.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://jsa.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://zon.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://cip.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ymj.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nzi.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://chn.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://lsk.shzxlz.cn

[F06] 删除文件
来源：http://qyx.aizwys.cn

Py:   os.remove("a.txt")
来源：http://ngy.yvedp.cn

PHP:  unlink("a.txt");
来源：http://mcy.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://soq.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://spa.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yuj.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://lzn.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://kds.cashguo.top

C#:   File.Delete("a.txt");
来源：http://qek.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://acu.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bxg.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mjp.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fuu.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://obt.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dag.andypj.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://llu.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vls.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://leb.cheryme.top

[F08] 遍历目录
来源：http://nnt.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dav.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bmy.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://opl.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://ryi.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://emv.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ymq.aizwys.cn

Ruby: Dir.children("dir")
来源：http://jsl.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://qtu.gogol.net.cn

[F09] 获取文件大小
来源：http://osk.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://rae.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://rfo.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://stp.chenlongwang.top

TS:   fs.statSync("a.txt").size
来源：http://qce.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cwt.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ywo.andypj.xyz

Ruby: File.size("a.txt")
来源：http://dpz.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://fce.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://mdu.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jqw.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bkr.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hpm.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://jur.yuanzhike.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wew.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vml.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://krm.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zdt.jianghu66.top

[F11] 复制与移动文件
来源：http://zqw.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fih.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iqy.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://thg.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gop.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xhn.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uld.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ycm.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kdr.yonumen.top

[F12] CSV 读写
来源：http://sag.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zpk.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ilv.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fdv.dashuyun.cn

TS:   // 同上
来源：http://qkm.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://txx.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jfd.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hpo.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uak.yuanzhike.top


<!-- 参考信息 -->