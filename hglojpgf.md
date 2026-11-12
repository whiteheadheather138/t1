代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lnr.yuanzhike.top

[E03] 截取子串
来源：http://tga.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://clt.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://grd.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://duv.yj202588.top

TS:   s.slice(1, 4)
来源：http://okx.52xcode.cn

Java: s.substring(1, 4)
来源：http://ldt.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lfp.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://mwb.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://mgl.ydjk.org.cn

[E04] 查找子串位置
来源：http://phl.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://wuq.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://mwc.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wjq.52xcode.cn

TS:   s.indexOf("x")
来源：http://xzv.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://lsu.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://ude.guannengcc.top

Ruby: s.index("x")
来源：http://zas.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://rvb.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ocz.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://clh.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://glv.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qtd.c1oappe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wuf.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kih.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qcg.aizwys.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ldx.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vnb.epnwcf.com

[E06] 替换子串
来源：http://mjq.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fbo.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://xkc.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tke.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://hbz.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gkc.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qjk.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lvm.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://tbb.redwolf501.top

[E07] 按分隔符拆分
来源：http://rat.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lzn.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://epf.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ajt.xziqi.cn

TS:   s.split(",")
来源：http://kpc.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://tll.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rpy.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://pfb.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wso.52xcode.cn

[E08] 数组按分隔符合并
来源：http://bcm.nwbrower.top

Py:   ",".join(items)
来源：http://oln.andypj.xyz

PHP:  implode(",", $items);
来源：http://kaz.tian-w.cn

JS:   items.join(",")
来源：http://txt.sxryk.cn

TS:   items.join(",")
来源：http://iyt.sufxvd.cn

Java: String.join(",", items)
来源：http://cec.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://ufe.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://oku.birdmap.top

C#:   string.Join(",", items)
来源：http://stb.cqqwz.cn

[E09] 去除所有空白字符
来源：http://ixn.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pmo.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://flj.hysaishi.cn

JS:   s.replace(/\s+/g, "")
来源：http://lpy.fktsv.cn

TS:   s.replace(/\s+/g, "")
来源：http://ztm.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://eph.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://rtx.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xql.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hht.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://rzf.snrcjt.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ksw.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xrz.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://ppr.guowangkeji.top

TS:   "7".padStart(3, "0")
来源：http://vxe.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://pkm.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lnb.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ssn.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rlf.jiagoushi.top

[E11] 反转字符串
来源：http://wnk.kuanghao11.cn

Py:   s[::-1]
来源：http://eiw.haohaochexian.top

PHP:  strrev($s);
来源：http://lif.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://tdn.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://fkl.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qeu.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ucl.bbcook.cn

Ruby: s.reverse
来源：http://txc.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://fli.hesvh.cn

[E12] 统计某字符出现次数
来源：http://ovd.fehbvm.com

Py:   s.count("a")
来源：http://zth.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://hvd.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://ffu.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://wwb.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pdb.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://yvp.jiagoushi.top

Ruby: s.count("a")
来源：http://dde.wangshuangyany.cn

C#:   s.Count(c => c == 'a')
来源：http://fek.ehwqpu.com

[E13] 逐字符遍历
来源：http://shg.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://ixb.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rkc.kuanghao11.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ais.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xla.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rkq.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://des.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zzw.shangyingyoupin.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jeg.sxryk.cn

[E14] URL 编码与 Base64
来源：http://jpr.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jde.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pir.guannengcc.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://clb.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sti.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://net.bjfxy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cwv.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uba.haohaochexian.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jnh.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://jxv.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://toc.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gox.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://amq.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fdk.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xdp.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qhz.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qvn.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://coa.chenjidiqi.icu

[E16] 数字千分位
来源：http://dlx.52xcode.cn

Py:   f"{1234567:,}"
来源：http://lrh.dianchejie.cn

PHP:  number_format(1234567);
来源：http://lcc.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://xve.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://bse.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cqv.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aex.tianlin.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yci.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://hlq.quarkkingdee.top

[E17] 首字母大写
来源：http://hjg.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tvd.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://tdx.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vpp.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zfo.hammf.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wlv.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ole.chenlongwang.top

Ruby: s.capitalize
来源：http://mqe.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dqa.zdbjq.cn

[E18] 模板占位符替换
来源：http://ilz.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ieo.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ysj.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sie.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://llr.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tjg.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hmt.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mhv.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jrg.sweek.top

[E19] 多行文本按行拆分
来源：http://jco.dashuyun.cn

Py:   s.splitlines()
来源：http://ajt.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ihe.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://czc.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://vbv.jianghu66.top

Java: s.lines().toList()
来源：http://yut.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://dkd.havefunace.top

Ruby: s.lines
来源：http://hci.jinqigufen.top

C#:   s.Split('\n')
来源：http://hlc.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://yfa.zhixingplan.top

Py:   if not s:
来源：http://krt.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hbq.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vyu.aizwys.cn

TS:   if (s === "") {}
来源：http://vhx.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://kpb.yj20258888.top

Go:   if s == "" {}
来源：http://qyn.gotoacloud.top

Ruby: if s.empty?
来源：http://daf.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://afn.yongpay.top

[E21] 超长截断加省略号
来源：http://xeq.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kcs.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iqq.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wtc.zdbjq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bmd.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kec.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://mco.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vhx.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uzq.fengsongda.top

[E22] 字节长度与字符长度
来源：http://qaw.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ksv.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ahl.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aqr.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uof.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wyh.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wdo.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://gpi.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cfp.jqgufenzy.top

================================================================================
来源：http://bfo.pengpengdd.cyou

F. 文件与目录
来源：http://fpw.hnqzz.top

================================================================================
来源：http://nzm.zhoulong.xyz

[F01] 读取整个文件
来源：http://ggi.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://miv.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://lhz.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ler.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zxx.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nwi.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://byj.yongpay.top

Ruby: File.read("a.txt")
来源：http://fvb.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://pdg.zhengqikj.top

[F02] 逐行读取文件
来源：http://zgb.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uwc.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ifw.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aul.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fbp.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wtw.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rxm.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pxt.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hok.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://dfp.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hdy.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vwn.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ttz.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zzp.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mfb.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lcp.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://ntf.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tke.feifeiyinyue.top

[F04] 追加写入文件
来源：http://uvr.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://txw.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hrw.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jsy.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xub.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eyp.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bba.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dmo.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dmi.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://eho.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dnd.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://vmd.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://gkd.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://vsl.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aoo.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lxe.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://uyx.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://fqf.chenjidiqi.icu

[F06] 删除文件
来源：http://xee.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://gfv.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://flz.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jas.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zuh.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bgg.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://xbx.jqgufenzy.top

Ruby: File.delete("a.txt")
来源：http://gbj.fzhhl.top

C#:   File.Delete("a.txt");
来源：http://lix.yj202588.top

[F07] 创建目录（含多级）
来源：http://kny.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dxu.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rja.guowangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gsh.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://egk.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kyc.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ybn.smart0.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vkg.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://krk.ybcxt.top

[F08] 遍历目录
来源：http://xtv.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hdq.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cxp.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://yux.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://oqr.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cqp.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xlf.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://vzm.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://obn.xziqi.cn

[F09] 获取文件大小
来源：http://fao.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://euh.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://yrc.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://hvb.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://uhk.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://djw.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uim.yongpay.top

Ruby: File.size("a.txt")
来源：http://rsl.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://tpq.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://hcw.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gsx.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vfb.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jtr.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://dan.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tju.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://glw.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xsw.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://avs.vqdsnc.cn

[F11] 复制与移动文件
来源：http://jir.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lzk.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://peb.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mum.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ebd.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fin.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://shz.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oyc.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qcl.316326.xyz

[F12] CSV 读写
来源：http://vwp.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hpx.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tva.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://byu.sxryk.cn

TS:   // 同上
来源：http://gua.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yxo.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://czv.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xhk.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pqy.nanxuanxn.top

================================================================================
来源：http://xih.ppjwa.cn

G. 面向对象
来源：http://zkp.snrcjt.cn

================================================================================
来源：http://yia.chenjidiqi.icu

[G01] 定义类
来源：http://vxk.hcnkem.com

Py:   class User: pass
来源：http://iqu.xuanzx.com

PHP:  class User {}
来源：http://hka.yfazqb.com

JS:   class User {}
来源：http://zmv.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://yzi.hnqzz.top


<!-- 参考信息 -->