代发 wailian999

TS:   "ab".repeat(3)
来源：http://ckh.zhoulong.xyz

Java: "ab".repeat(3)
来源：http://oez.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://rxv.c1oappe.top

Ruby: "ab" * 3
来源：http://ggk.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zsw.yonumen.top

[E03] 截取子串
来源：http://pup.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ypc.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zlc.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dud.zdqjudy.top

TS:   s.slice(1, 4)
来源：http://exy.jiagoushi.top

Java: s.substring(1, 4)
来源：http://htn.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dhs.shanyushiyangtech.top

Ruby: s[1, 3];  s[1..3]
来源：http://tzf.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://lrp.hongshengwenyu.top

[E04] 查找子串位置
来源：http://ubm.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://iuk.smart0.xyz

PHP:  strpos($s, "x");
来源：http://iyi.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pix.havefunace.top

TS:   s.indexOf("x")
来源：http://scp.zhoulong.xyz

Java: s.indexOf("x")
来源：http://veu.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://dwn.yvedp.cn

Ruby: s.index("x")
来源：http://vqn.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://rfu.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yxp.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://udy.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lja.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ncf.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://eqh.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jux.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vmp.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ngx.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vkg.feifeiyinyue.top

[E06] 替换子串
来源：http://qoo.zdqjudy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://era.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://lrj.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tyw.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://ffu.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://elq.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://azm.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lmt.redwolf501.top

C#:   s.Replace("a", "b")
来源：http://ghg.yfazqb.com

[E07] 按分隔符拆分
来源：http://yka.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tcd.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://odv.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zux.cashguo.top

TS:   s.split(",")
来源：http://wau.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://bcu.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vqj.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://qjn.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zms.shuidangran.top

[E08] 数组按分隔符合并
来源：http://rnz.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://aox.yuxming.cn

PHP:  implode(",", $items);
来源：http://xml.zhongyouzk.top

JS:   items.join(",")
来源：http://koo.xylfe.cn

TS:   items.join(",")
来源：http://ogv.gzhubu.top

Java: String.join(",", items)
来源：http://ymw.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://hrb.yj202588.top

Ruby: items.join(",")
来源：http://cty.hywenlv.cn

C#:   string.Join(",", items)
来源：http://nwq.aizwys.cn

[E09] 去除所有空白字符
来源：http://chv.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nit.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eza.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://qgs.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://mfi.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://typ.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wsb.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hbv.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vrn.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://jyc.yueranfly.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://obq.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ztd.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://neb.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://dlx.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://kvw.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://agm.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xov.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lxj.nanxinkj.top

[E11] 反转字符串
来源：http://sgb.zdbjq.cn

Py:   s[::-1]
来源：http://res.gzhubu.top

PHP:  strrev($s);
来源：http://dws.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://igc.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://bqm.9152youxi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fyv.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rbg.guannengcc.top

Ruby: s.reverse
来源：http://led.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://zfi.cucudq.cn

[E12] 统计某字符出现次数
来源：http://yma.meibo888.top

Py:   s.count("a")
来源：http://vzz.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://cbz.havefunace.top

JS:   s.split("a").length - 1
来源：http://mez.316326.xyz

TS:   s.split("a").length - 1
来源：http://lvf.pengpengdd.cyou

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ryw.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://uxk.hfpthk.cn

Ruby: s.count("a")
来源：http://ihk.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://odd.sjlbkw.cn

[E13] 逐字符遍历
来源：http://ioo.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://qjv.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ivw.xylfe.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://crf.vehdjk.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://mem.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vuf.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kkn.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://krw.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zeb.sxryk.cn

[E14] URL 编码与 Base64
来源：http://ppo.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://caz.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://uat.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ucj.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oyv.yj202588.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zsu.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qwf.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vha.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kpq.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://ond.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://knz.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mnr.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qdh.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ofx.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ior.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://odq.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cvb.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hcc.sjlbkw.cn

[E16] 数字千分位
来源：http://yax.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://tjh.yongpay.top

PHP:  number_format(1234567);
来源：http://aud.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oea.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zku.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xtf.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nsz.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wdi.ywan-chungtsiang.top

C#:   1234567.ToString("N0")
来源：http://haa.aibaodan.cn

[E17] 首字母大写
来源：http://xjd.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mbt.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bjd.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ovi.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://arr.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rgk.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zgv.guowangkeji.top

Ruby: s.capitalize
来源：http://ivl.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mlr.bjfxy.top

[E18] 模板占位符替换
来源：http://nqh.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gze.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vtn.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://juo.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://inu.chenlongwang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://veq.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nin.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zcq.pengpengdd.cyou

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xko.tian-w.cn

[E19] 多行文本按行拆分
来源：http://fxl.cdnleiting.top

Py:   s.splitlines()
来源：http://rbm.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uck.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://tuj.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://ism.jqgfzy.top

Java: s.lines().toList()
来源：http://gqq.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://nqw.zdqjudy.top

Ruby: s.lines
来源：http://gjt.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://uqe.redwolf501.top

[E20] 判断字符串是否为空
来源：http://mhe.zhaomingkeji.xyz

Py:   if not s:
来源：http://gut.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bwr.hnqzz.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ceg.fengsongda.top

TS:   if (s === "") {}
来源：http://gus.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://log.cashguo.top

Go:   if s == "" {}
来源：http://xef.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://xvm.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qkk.dashuyun.cn

[E21] 超长截断加省略号
来源：http://oqp.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vlx.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://siz.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jcb.bjfxy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezi.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zit.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://byl.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dap.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eqd.c1oappe.top

[E22] 字节长度与字符长度
来源：http://nxx.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wde.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://een.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sth.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ida.316326.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lov.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lux.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://zjx.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qex.ppjwa.cn

================================================================================
来源：http://oea.redwolf501.top

F. 文件与目录
来源：http://zke.gotoacloud.top

================================================================================
来源：http://xuf.nwbrower.top

[F01] 读取整个文件
来源：http://yxw.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jxy.daria6918.cn

PHP:  file_get_contents("a.txt");
来源：http://zpg.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mks.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ntq.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://erk.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fga.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://yyk.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://gpf.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://bom.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hef.tian-w.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cgf.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dsu.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vzg.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cri.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lpk.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wli.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sij.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://hic.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gyp.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://llb.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://axz.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gth.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gac.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://luu.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://zvp.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xuv.zhixingplan.top

[F04] 追加写入文件
来源：http://vxo.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rqo.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uur.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rra.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fzj.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vut.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://awo.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rgy.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pbj.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://jpm.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mkq.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://lrd.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://hqq.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://kru.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bar.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nqy.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://mmt.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://xgs.shangyingyoupin.top

[F06] 删除文件
来源：http://uxm.yj202588.top

Py:   os.remove("a.txt")
来源：http://yui.epnwcf.com

PHP:  unlink("a.txt");
来源：http://zdp.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://yta.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://cey.jlsjyb.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dub.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://cez.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://uyu.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://qzg.mhx1999.top

[F07] 创建目录（含多级）
来源：http://mua.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hrm.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rnq.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hql.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://syb.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cxt.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://klf.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fyb.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pvk.haohaochexian.top

[F08] 遍历目录
来源：http://zuv.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://kzq.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mem.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://ken.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://qdw.hongshengwenyu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cmp.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://anx.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://seu.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://bil.wangshuangyany.cn

[F09] 获取文件大小
来源：http://plb.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://hxg.yueranfly.top

PHP:  filesize("a.txt");
来源：http://rkh.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://sss.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://hzq.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bjd.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://twt.cucudq.cn

Ruby: File.size("a.txt")
来源：http://pxg.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://lfo.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://fxy.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ulf.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mvl.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://onb.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://wtt.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hwh.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://poi.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aga.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pyu.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://hqu.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qdr.yuxming.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vti.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cne.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xev.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fad.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fgd.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rpi.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://prw.hnxiangtu.top

[F12] CSV 读写
来源：http://loi.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://enp.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://azi.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://obn.ybcxt.top

TS:   // 同上
来源：http://ltf.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vef.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mnb.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fip.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://jtn.andypj.xyz

================================================================================
来源：http://ufz.bbcook.cn

G. 面向对象
来源：http://yqm.yj20258.top

================================================================================
来源：http://sav.xuetiantiany.cn

[G01] 定义类
来源：http://tuk.jinqigufen.top


<!-- 参考信息 -->