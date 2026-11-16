代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eic.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ynb.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aix.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dwe.jinqigufen.top

[E02] 重复字符串
来源：http://gvp.gotoacloud.top

Py:   "ab" * 3
来源：http://csb.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://cfy.cashguo.top

JS:   "ab".repeat(3)
来源：http://ilu.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://mji.iojbl.cn

Java: "ab".repeat(3)
来源：http://duu.zhaomingkeji.xyz

Go:   strings.Repeat("ab", 3)
来源：http://isb.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://lqi.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ram.shanyushiyangkeji.top

[E03] 截取子串
来源：http://oqx.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vde.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pml.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vbz.wangdashe.top

TS:   s.slice(1, 4)
来源：http://iis.fktsv.cn

Java: s.substring(1, 4)
来源：http://vvw.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uct.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://pah.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://ujd.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://xwj.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://trt.epnwcf.com

PHP:  strpos($s, "x");
来源：http://git.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://huy.nanxinkj.top

TS:   s.indexOf("x")
来源：http://uhg.nanxinkj.top

Java: s.indexOf("x")
来源：http://glw.jqgfzy.top

Go:   strings.Index(s, "x")
来源：http://lru.nwbrower.top

Ruby: s.index("x")
来源：http://amu.mhx1999.top

C#:   s.IndexOf("x")
来源：http://fjt.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mce.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hxq.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://udb.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bzb.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lvm.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nsw.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jpb.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fgw.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xpx.daria6918.cn

[E06] 替换子串
来源：http://efg.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://van.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://vka.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nyh.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://uts.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ivi.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://shl.mhx1999.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lxy.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://plg.chenlongwang.top

[E07] 按分隔符拆分
来源：http://kug.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kze.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dkz.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://dha.daxiang520.top

TS:   s.split(",")
来源：http://nny.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://rty.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://flz.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://xld.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rpx.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://gnj.zhijiandao.cn

Py:   ",".join(items)
来源：http://gav.daxiang520.top

PHP:  implode(",", $items);
来源：http://ogs.xziqi.cn

JS:   items.join(",")
来源：http://tyz.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://gvh.pengpengdd.cyou

Java: String.join(",", items)
来源：http://gou.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://rpl.shuidangran.top

Ruby: items.join(",")
来源：http://lwu.svipenyu.cn

C#:   string.Join(",", items)
来源：http://zjf.sxryk.cn

[E09] 去除所有空白字符
来源：http://mwl.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fja.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ibq.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://lia.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://vul.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://kux.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lep.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hkp.sysykeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ggt.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://gmi.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bob.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fna.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://lsb.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://sfj.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://iwy.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://fzb.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sjr.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://efi.yueranfly.top

[E11] 反转字符串
来源：http://ixj.fzhhl.top

Py:   s[::-1]
来源：http://ptj.sjlbkw.cn

PHP:  strrev($s);
来源：http://qmf.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://gnf.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://yvd.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yom.zhaomingkeji.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ngl.jianghu66.top

Ruby: s.reverse
来源：http://map.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fkp.zhaomingkeji.xyz

[E12] 统计某字符出现次数
来源：http://ayj.hcnkem.com

Py:   s.count("a")
来源：http://eif.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://gnw.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://blb.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://vxf.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bbx.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://nbz.smart0.xyz

Ruby: s.count("a")
来源：http://aqa.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://pci.hywenlv.cn

[E13] 逐字符遍历
来源：http://uql.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://wxo.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dkz.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nnz.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gqh.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rrg.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fqh.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rjg.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ldw.uphjek.com

[E14] URL 编码与 Base64
来源：http://gnv.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mxo.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kob.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bxj.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iry.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://boo.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://clq.hongshengwenyu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dsu.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ven.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://nyc.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bxj.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wzi.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tpn.xuetiantiany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mlq.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vtf.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://goh.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://erm.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ehw.yanxiufei.cn

[E16] 数字千分位
来源：http://iiw.yj20258.top

Py:   f"{1234567:,}"
来源：http://pmv.yonumen.top

PHP:  number_format(1234567);
来源：http://uxc.yfazqb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://yug.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lwd.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zxd.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jvo.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bpm.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://vlq.tianlin.xyz

[E17] 首字母大写
来源：http://yde.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bqz.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://iqn.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pxy.yanxiufei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hcu.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qul.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vhi.jiagoushi.top

Ruby: s.capitalize
来源：http://lvb.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kpe.haohaochexian.top

[E18] 模板占位符替换
来源：http://wus.daria6918.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qoh.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nqv.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://jai.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sny.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xgb.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kmn.andypj.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rlu.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dew.316326.xyz

[E19] 多行文本按行拆分
来源：http://feu.fehbvm.com

Py:   s.splitlines()
来源：http://afu.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qbf.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://rgx.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://ugh.wangshuangyany.cn

Java: s.lines().toList()
来源：http://zqg.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://izg.yonumen.top

Ruby: s.lines
来源：http://uvd.andypj.xyz

C#:   s.Split('\n')
来源：http://hkr.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://eea.tarul.cn

Py:   if not s:
来源：http://fwo.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ecd.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fcx.hysaishi.cn

TS:   if (s === "") {}
来源：http://nja.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://uhb.wangshuangyany.cn

Go:   if s == "" {}
来源：http://qwn.gotoacloud.top

Ruby: if s.empty?
来源：http://stq.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xve.tian-w.cn

[E21] 超长截断加省略号
来源：http://tan.hnxiangtu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pud.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bew.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ybn.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xnu.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yrs.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://pwi.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yjf.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hfs.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://fau.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xyz.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ded.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uag.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tls.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rxa.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bwf.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://uvl.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kzs.epnwcf.com

================================================================================
来源：http://mok.uphjek.com

F. 文件与目录
来源：http://wbe.tianlin.xyz

================================================================================
来源：http://zmq.bbcook.cn

[F01] 读取整个文件
来源：http://qhs.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pjf.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://sjb.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iwm.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ckn.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cgw.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wgh.tianlin.xyz

Ruby: File.read("a.txt")
来源：http://pxe.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://lst.hcnkem.com

[F02] 逐行读取文件
来源：http://pcv.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nms.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ewo.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gvn.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bbw.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://svu.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wtn.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bbu.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://srh.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://vvg.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mvi.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xwj.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://taf.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yjy.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ifm.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wcl.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://mqb.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jfv.dashuyun.cn

[F04] 追加写入文件
来源：http://oan.cucudq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gbp.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://swo.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://csn.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wey.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vmh.wangdashe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ody.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dzq.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rwe.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://waj.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dpe.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://cfy.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://eib.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://vtg.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ifg.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cft.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://qxb.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://ykp.quarkkingdee.top

[F06] 删除文件
来源：http://bea.meibo888.top

Py:   os.remove("a.txt")
来源：http://etf.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://iry.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://dwj.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uvb.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vyw.havefunace.top

Go:   os.Remove("a.txt")
来源：http://ouu.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://jgx.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://xhf.ydzc1.top

[F07] 创建目录（含多级）
来源：http://dvt.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eoh.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xzj.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lci.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://weg.epnwcf.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ndi.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wdd.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hxz.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ygr.bbcook.cn

[F08] 遍历目录
来源：http://fat.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dbw.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nyh.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://gbz.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://tqj.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hhr.yj20258.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qwb.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://nib.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://zid.zhiwuduotai.top

[F09] 获取文件大小
来源：http://oip.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://our.xziqi.cn

PHP:  filesize("a.txt");
来源：http://sny.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://wrj.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://kng.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://hqc.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://udn.yuxming.cn

Ruby: File.size("a.txt")
来源：http://zkl.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://qlu.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://etl.fehbvm.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://awq.uphjek.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ohi.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://esg.smart0.xyz

TS:   path.extname("a.txt")
来源：http://cpc.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kpj.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kmn.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oav.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://scc.ehwqpu.com

[F11] 复制与移动文件
来源：http://swr.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pup.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jou.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bmq.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ikz.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://flj.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zov.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pvl.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iga.jqgfzy.top

[F12] CSV 读写
来源：http://qdp.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bun.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wgp.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dpj.mhx1999.top

TS:   // 同上
来源：http://lfv.zhoulong.xyz


<!-- 参考信息 -->