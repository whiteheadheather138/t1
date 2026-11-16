代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dxz.hesvh.cn

[E03] 截取子串
来源：http://sjz.havefunace.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vpe.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aki.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eac.fengsongda.top

TS:   s.slice(1, 4)
来源：http://yzr.cashguo.top

Java: s.substring(1, 4)
来源：http://jvs.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qhy.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://khq.tarul.cn

C#:   s.Substring(1, 3)
来源：http://fcc.ehwqpu.com

[E04] 查找子串位置
来源：http://tyq.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://nch.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://zus.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gch.jyoumei.cn

TS:   s.indexOf("x")
来源：http://ptq.svipenyu.cn

Java: s.indexOf("x")
来源：http://rnm.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://rhy.hysaishi.cn

Ruby: s.index("x")
来源：http://sid.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://ukj.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ovs.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dtm.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rxg.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fea.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://csg.yj20258.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fmf.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mud.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://adc.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zdd.shzxlz.cn

[E06] 替换子串
来源：http://hxo.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://udd.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://wvw.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oir.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://lui.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tqt.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ycd.hywenlv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dmm.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://crl.cashguo.top

[E07] 按分隔符拆分
来源：http://fba.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://min.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pza.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ofb.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://xco.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://goo.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ydx.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://qyi.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://spi.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://oxl.haohaochexian.top

Py:   ",".join(items)
来源：http://vhz.yvedp.cn

PHP:  implode(",", $items);
来源：http://afr.daxiang520.top

JS:   items.join(",")
来源：http://cbj.jinghuilouyu.cn

TS:   items.join(",")
来源：http://fqi.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://yju.aibaodan.cn

Go:   strings.Join(items, ",")
来源：http://ucu.nanxinkj.top

Ruby: items.join(",")
来源：http://zki.nanxinkj.top

C#:   string.Join(",", items)
来源：http://ozn.dashuyun.cn

[E09] 去除所有空白字符
来源：http://oax.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dab.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qco.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://ykx.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://lgy.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://jsm.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gni.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://umk.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qbx.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://dhv.sxryk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://stt.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wqf.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://red.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://dli.epnwcf.com

Java: String.format("%03d", 7)
来源：http://imd.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://aox.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hsc.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ymy.chenzaomai.com

[E11] 反转字符串
来源：http://tsk.fanxiaobao.xyz

Py:   s[::-1]
来源：http://lwp.yonumen.top

PHP:  strrev($s);
来源：http://xqg.hammf.cn

JS:   [...s].reverse().join("")
来源：http://nru.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://heg.jyoumei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tdh.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nrp.xingfuxueyuan.xyz

Ruby: s.reverse
来源：http://kko.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lrn.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://guc.0kj1m.cn

Py:   s.count("a")
来源：http://fic.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://gyf.fehbvm.com

JS:   s.split("a").length - 1
来源：http://imo.bjfxy.top

TS:   s.split("a").length - 1
来源：http://buc.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hkt.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://rgt.daxiang520.top

Ruby: s.count("a")
来源：http://wjy.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://iks.fengsongda.top

[E13] 逐字符遍历
来源：http://ulw.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://dar.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jkj.xylfe.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lqd.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kdi.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gcj.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cxn.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nlj.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kfy.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://pkc.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hav.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ure.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lfi.bjfxy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pgn.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aoo.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://roe.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fcw.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zuo.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://ycj.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lyi.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gsv.fzhhl.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pen.9152youxi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pgb.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tps.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qpy.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jlv.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lfj.xuanzx.com

[E16] 数字千分位
来源：http://ytr.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://vyp.dianchejie.cn

PHP:  number_format(1234567);
来源：http://mvn.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://cfw.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hye.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mzf.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qkb.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ynj.uphjek.com

C#:   1234567.ToString("N0")
来源：http://esk.ehwqpu.com

[E17] 首字母大写
来源：http://skc.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://avy.0kj1m.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uyk.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wtb.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nuf.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eiv.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fhv.zdqjudy.top

Ruby: s.capitalize
来源：http://voe.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cpx.hesvh.cn

[E18] 模板占位符替换
来源：http://ovr.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kyk.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bwo.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wad.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nuj.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oqh.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ykb.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rqt.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pio.ydzc1.top

[E19] 多行文本按行拆分
来源：http://sqk.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://ymg.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wvk.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://toa.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://iyv.cashguo.top

Java: s.lines().toList()
来源：http://zal.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://gsx.hammf.cn

Ruby: s.lines
来源：http://zzl.mhx1999.top

C#:   s.Split('\n')
来源：http://xfw.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://mmc.0kj1m.cn

Py:   if not s:
来源：http://hqm.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wvb.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ixz.hcnkem.com

TS:   if (s === "") {}
来源：http://zwv.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://rhy.yongpay.top

Go:   if s == "" {}
来源：http://lfw.vqdsnc.cn

Ruby: if s.empty?
来源：http://nzp.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xnb.cdnleiting.top

[E21] 超长截断加省略号
来源：http://zgw.zhixingplan.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bbm.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://brg.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xuu.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wsi.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mxw.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://kxg.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zix.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ezj.cheryme.top

[E22] 字节长度与字符长度
来源：http://iaw.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://axw.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lip.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xvd.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blx.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iyi.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://znu.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://anu.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hzo.daria6918.cn

================================================================================
来源：http://fpc.jqgfzy.top

F. 文件与目录
来源：http://msk.bbcook.cn

================================================================================
来源：http://dnw.0kj1m.cn

[F01] 读取整个文件
来源：http://whp.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sye.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://mlj.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://afl.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://udo.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://alb.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nme.pycfn.com

Ruby: File.read("a.txt")
来源：http://pzp.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://yzy.c1oappe.top

[F02] 逐行读取文件
来源：http://aam.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wmx.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wfy.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tnk.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pxm.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xle.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xwb.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fgw.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pbp.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://rkl.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://czn.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://txc.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yhx.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oud.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://klu.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vue.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://spk.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wzy.xinyue.icu

[F04] 追加写入文件
来源：http://yix.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ayy.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://toi.hesvh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ard.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vaw.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kle.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jhz.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ouv.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://env.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://rwc.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ytt.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://koo.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://aei.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://igz.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kpj.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uuf.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://oqn.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://tfc.guannengcc.top

[F06] 删除文件
来源：http://fie.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://zun.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://zbt.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://muk.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://zsr.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wcr.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://lyl.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://oym.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://ntn.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://tkx.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ivu.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xcq.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://owp.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fkz.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nkv.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zkl.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eix.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yqa.xziqi.cn

[F08] 遍历目录
来源：http://aar.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://anw.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bhz.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://egj.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://lcl.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kxb.fktsv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yeh.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://xqz.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://gbs.chenzaomai.com

[F09] 获取文件大小
来源：http://rza.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://bzf.cheryme.top

PHP:  filesize("a.txt");
来源：http://fbw.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://wbg.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://ltk.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://jrl.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xwc.yj202588.top

Ruby: File.size("a.txt")
来源：http://ovy.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://tdo.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://jsn.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ykh.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jjt.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ppm.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://tsh.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bok.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cku.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mwe.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://edr.zhoulong.xyz

[F11] 复制与移动文件
来源：http://jmw.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ppu.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jhe.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aea.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pec.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dgj.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nix.vehdjk.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://luj.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pbr.yj20258888.top

[F12] CSV 读写
来源：http://bxo.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tpi.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fjg.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wgj.zdqjudy.top

TS:   // 同上
来源：http://ndq.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ldv.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xjf.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qyh.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dif.birdmap.top

================================================================================
来源：http://dno.nanxinkj.top

G. 面向对象
来源：http://frz.ydzc1.top

================================================================================
来源：http://qbp.hysaishi.cn

[G01] 定义类
来源：http://hob.hywenlv.cn

Py:   class User: pass
来源：http://nam.ywan-chungtsiang.top

PHP:  class User {}
来源：http://cxd.redwolf501.top

JS:   class User {}
来源：http://lfo.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://yxr.hcnkem.com


<!-- 参考信息 -->