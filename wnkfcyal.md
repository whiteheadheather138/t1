代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ufh.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sba.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://swh.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jox.zhiwuduotai.top

[E02] 重复字符串
来源：http://lpi.quarkkingdee.top

Py:   "ab" * 3
来源：http://tua.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://hjo.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://jhk.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://aif.tianlin.xyz

Java: "ab".repeat(3)
来源：http://fav.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://gfn.redwolf501.top

Ruby: "ab" * 3
来源：http://anr.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cxy.fktsv.cn

[E03] 截取子串
来源：http://sgj.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lnp.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://niz.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yeu.cashguo.top

TS:   s.slice(1, 4)
来源：http://pdk.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://hmk.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tye.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://yis.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://hze.hesvh.cn

[E04] 查找子串位置
来源：http://hyi.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://eqr.meibo888.top

PHP:  strpos($s, "x");
来源：http://nsh.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rwv.fengsongda.top

TS:   s.indexOf("x")
来源：http://jzc.nanxuanxn.top

Java: s.indexOf("x")
来源：http://umh.yuxming.cn

Go:   strings.Index(s, "x")
来源：http://gzp.zhengqikj.top

Ruby: s.index("x")
来源：http://cvu.yj20258888.top

C#:   s.IndexOf("x")
来源：http://ihl.hcnkem.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://fji.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wbj.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ean.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wln.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ptj.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kjs.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wyc.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pjm.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://puy.sweek.top

[E06] 替换子串
来源：http://tzj.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vkd.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://jgx.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ksy.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://vbk.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xkk.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bqp.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bai.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://nzn.wangdashe.top

[E07] 按分隔符拆分
来源：http://dnw.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gym.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://njm.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://kzr.svipenyu.cn

TS:   s.split(",")
来源：http://bdn.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://anq.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qxr.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://uhb.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ihy.mhx1999.top

[E08] 数组按分隔符合并
来源：http://mak.andypj.xyz

Py:   ",".join(items)
来源：http://gxb.vehdjk.com

PHP:  implode(",", $items);
来源：http://qli.bjfxy.top

JS:   items.join(",")
来源：http://inp.gotoacloud.top

TS:   items.join(",")
来源：http://ggh.feifeiyinyue.top

Java: String.join(",", items)
来源：http://ldf.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://dcb.yuxming.cn

Ruby: items.join(",")
来源：http://lna.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://qdr.tarul.cn

[E09] 去除所有空白字符
来源：http://hwh.sysykeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hfp.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vbe.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://ilf.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://vvy.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://dyu.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jxk.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://rdp.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://crq.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://vnq.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xgr.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hba.sweek.top

JS:   "7".padStart(3, "0")
来源：http://uyo.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://jxr.vqdsnc.cn

Java: String.format("%03d", 7)
来源：http://cnb.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xme.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gdr.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mfj.shanyushiyangtech.top

[E11] 反转字符串
来源：http://cbh.zycfv.cn

Py:   s[::-1]
来源：http://zpt.chenlongwang.top

PHP:  strrev($s);
来源：http://jrv.cheryme.top

JS:   [...s].reverse().join("")
来源：http://jxs.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://fto.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://din.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://flg.gotoacloud.top

Ruby: s.reverse
来源：http://acd.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nuk.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://fvj.yueranfly.top

Py:   s.count("a")
来源：http://ykk.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://pmf.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://jdf.aizwys.cn

TS:   s.split("a").length - 1
来源：http://emw.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mwm.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://qqn.jqgfzy.top

Ruby: s.count("a")
来源：http://tct.chenzaomai.com

C#:   s.Count(c => c == 'a')
来源：http://ori.316326.xyz

[E13] 逐字符遍历
来源：http://jbl.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://jpb.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jjb.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gsf.hywenlv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://thm.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dbm.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jdy.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://cre.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://evs.hammf.cn

[E14] URL 编码与 Base64
来源：http://snu.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cwv.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://gok.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bwu.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vdi.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vii.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yjg.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tiq.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vyq.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://akm.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://esz.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uaf.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zow.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fjg.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dvk.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oqp.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hnf.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dsd.daria6918.cn

[E16] 数字千分位
来源：http://tjs.fzhhl.top

Py:   f"{1234567:,}"
来源：http://nxh.fzhhl.top

PHP:  number_format(1234567);
来源：http://gee.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ddt.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://trt.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ymu.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tns.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yno.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://dwl.9152youxi.cn

[E17] 首字母大写
来源：http://ruv.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ycv.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pvp.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bds.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ltc.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yrk.ybcxt.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bqn.sjlbkw.cn

Ruby: s.capitalize
来源：http://iqf.wangshuangyany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kre.xylfe.cn

[E18] 模板占位符替换
来源：http://xps.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zek.sjlbkw.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ank.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rdi.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gid.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ysx.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fvp.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hsp.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ddn.birdmap.top

[E19] 多行文本按行拆分
来源：http://zsd.xylfe.cn

Py:   s.splitlines()
来源：http://jvh.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cqv.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://iho.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://hdf.dianchejie.cn

Java: s.lines().toList()
来源：http://vgq.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://qvb.gaohongyu789.top

Ruby: s.lines
来源：http://qcs.tianlin.xyz

C#:   s.Split('\n')
来源：http://drc.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://jxa.cashguo.top

Py:   if not s:
来源：http://fcc.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pad.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sof.52xcode.cn

TS:   if (s === "") {}
来源：http://mzx.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://jna.kuanghao11.cn

Go:   if s == "" {}
来源：http://hzy.daria6918.cn

Ruby: if s.empty?
来源：http://kkh.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zsb.tanke756.top

[E21] 超长截断加省略号
来源：http://mkq.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qzt.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zas.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qev.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://osk.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zgp.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://hus.yonumen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uvg.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ztp.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://yoy.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://grs.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sra.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lup.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ify.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nub.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qjj.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://brv.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tmh.jiagoushi.top

================================================================================
来源：http://vfm.havefunace.top

F. 文件与目录
来源：http://cqf.gogol.net.cn

================================================================================
来源：http://brt.9152youxi.cn

[F01] 读取整个文件
来源：http://ujr.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qzl.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://xhl.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mik.quarkkingdee.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bqi.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qtt.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gsq.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://dia.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://yvq.uphjek.com

[F02] 逐行读取文件
来源：http://glm.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yed.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tid.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ddt.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vvy.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fuj.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wus.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jyx.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dpc.cheryme.top

[F03] 写入文件（覆盖）
来源：http://xle.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jpj.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lep.daxiang520.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zlo.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bik.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dfo.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cud.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://trl.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mgo.jlsjyb.cn

[F04] 追加写入文件
来源：http://air.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wwm.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://axc.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lat.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://puf.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sji.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xci.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nlz.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ymc.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://cmo.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kxc.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://ocr.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://bve.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://jdp.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wns.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aat.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://pyc.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://zes.jinqigfzy.top

[F06] 删除文件
来源：http://hmk.tarul.cn

Py:   os.remove("a.txt")
来源：http://cfn.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://wom.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://qwn.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://aal.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eft.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://gdq.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://swo.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://aoq.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://rrz.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sir.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bfq.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yes.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ywg.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pya.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sfe.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kpk.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nus.gaohongyu789.top

[F08] 遍历目录
来源：http://osn.hywenlv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vcr.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://orz.gogol.net.cn

JS:   fs.readdirSync("dir")
来源：http://xks.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://olv.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lus.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fhm.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://qwq.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://hlh.hysaishi.cn

[F09] 获取文件大小
来源：http://qcp.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://hth.wangdashe.top

PHP:  filesize("a.txt");
来源：http://afv.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://qdq.sysykeji.top

TS:   fs.statSync("a.txt").size
来源：http://anx.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://nja.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kvs.shuidangran.top

Ruby: File.size("a.txt")
来源：http://mls.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://koo.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://qni.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://guq.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jxz.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ohb.daria6918.cn

TS:   path.extname("a.txt")
来源：http://zmc.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rob.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rlb.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nrg.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gnd.aizwys.cn

[F11] 复制与移动文件
来源：http://vai.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mtu.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://goq.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qdy.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uur.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hlx.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dkb.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yny.zhoulong.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lnq.jinqigfzy.top

[F12] CSV 读写
来源：http://jaq.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wfi.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yab.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zuh.zdqjudy.top

TS:   // 同上
来源：http://hzd.xylfe.cn


<!-- 参考信息 -->