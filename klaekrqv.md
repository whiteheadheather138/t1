代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fah.zhijiandao.cn

[E03] 截取子串
来源：http://lzj.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wtr.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cxb.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mfo.yj20258.top

TS:   s.slice(1, 4)
来源：http://ati.haohaochexian.top

Java: s.substring(1, 4)
来源：http://snm.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tjy.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://msc.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://rey.cucudq.cn

[E04] 查找子串位置
来源：http://hdx.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://lrf.hesvh.cn

PHP:  strpos($s, "x");
来源：http://bjb.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gnx.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://gxp.havefunace.top

Java: s.indexOf("x")
来源：http://ung.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://kxd.yonumen.top

Ruby: s.index("x")
来源：http://biy.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://cgr.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vha.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nvf.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cyp.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lxu.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wwi.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fix.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rkd.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aqk.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zpp.jinghuilouyu.cn

[E06] 替换子串
来源：http://tbc.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wwb.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://jsa.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gox.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://hah.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lzx.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qcj.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vjw.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://wiz.svipenyu.cn

[E07] 按分隔符拆分
来源：http://lax.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xce.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zle.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bwm.vehdjk.com

TS:   s.split(",")
来源：http://jwj.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://prw.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ylv.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://hlm.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vzb.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://fbg.fengsongda.top

Py:   ",".join(items)
来源：http://doc.tanke756.top

PHP:  implode(",", $items);
来源：http://vks.yongpay.top

JS:   items.join(",")
来源：http://ikw.snrcjt.cn

TS:   items.join(",")
来源：http://qcg.zdqjudy.top

Java: String.join(",", items)
来源：http://dwy.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://cyw.hysaishi.cn

Ruby: items.join(",")
来源：http://rkt.ybcxt.top

C#:   string.Join(",", items)
来源：http://pcr.svipenyu.cn

[E09] 去除所有空白字符
来源：http://zyz.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gtn.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pux.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://srg.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://ukq.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://xqn.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dhp.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://aqr.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://usc.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://uli.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fht.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ulx.ybcxt.top

JS:   "7".padStart(3, "0")
来源：http://brt.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://raa.vehdjk.com

Java: String.format("%03d", 7)
来源：http://iiq.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://uwk.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wtm.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mfb.havefunace.top

[E11] 反转字符串
来源：http://mqi.guowangkeji.top

Py:   s[::-1]
来源：http://civ.hesvh.cn

PHP:  strrev($s);
来源：http://del.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://yya.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://uid.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vos.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://dpl.tarul.cn

Ruby: s.reverse
来源：http://rpo.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://dsw.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://key.chenlongwang.top

Py:   s.count("a")
来源：http://yjm.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://cck.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://nxp.daxiang520.top

TS:   s.split("a").length - 1
来源：http://xhk.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kso.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://ymx.sysykeji.top

Ruby: s.count("a")
来源：http://rmo.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://qov.dianchejie.cn

[E13] 逐字符遍历
来源：http://dqt.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://bhq.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ups.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://wam.yueranfly.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mnr.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://efv.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xpq.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mgz.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fak.tanke756.top

[E14] URL 编码与 Base64
来源：http://mga.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nid.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lwb.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fzl.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tly.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kws.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dst.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qwv.zdqjudy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vma.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://lzv.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uhr.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rah.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eud.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://urw.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bna.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tpc.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cru.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yvo.tanke756.top

[E16] 数字千分位
来源：http://ffm.tian-w.cn

Py:   f"{1234567:,}"
来源：http://pwx.yuanzhike.top

PHP:  number_format(1234567);
来源：http://zfp.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://lpk.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zfm.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zbi.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fup.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ovj.tarul.cn

C#:   1234567.ToString("N0")
来源：http://qzb.guannengcc.top

[E17] 首字母大写
来源：http://iam.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sba.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xki.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hzz.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qyf.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dhi.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qzy.xuetiantiany.cn

Ruby: s.capitalize
来源：http://ocu.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eiu.zhongyouzk.top

[E18] 模板占位符替换
来源：http://rqi.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eyv.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kmq.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ugh.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zkq.yueranfly.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kjk.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iad.shzxlz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eqd.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jgm.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://xto.birdmap.top

Py:   s.splitlines()
来源：http://ydo.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yer.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://ijb.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://nan.316326.xyz

Java: s.lines().toList()
来源：http://qdm.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://eva.dashuyun.cn

Ruby: s.lines
来源：http://wse.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://mkv.fktsv.cn

[E20] 判断字符串是否为空
来源：http://ejo.shangyingyoupin.top

Py:   if not s:
来源：http://hdb.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tbw.yfazqb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fcw.jyoumei.cn

TS:   if (s === "") {}
来源：http://flz.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://sli.tianlin.xyz

Go:   if s == "" {}
来源：http://mfb.daxiang520.top

Ruby: if s.empty?
来源：http://ibe.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cau.yvedp.cn

[E21] 超长截断加省略号
来源：http://cpi.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nor.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gyl.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kvw.shzxlz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xku.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lof.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://eua.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ucl.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rtx.meibo888.top

[E22] 字节长度与字符长度
来源：http://zlp.redwolf501.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kow.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yra.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wyl.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://btm.zdqjudy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cpq.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dyp.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://htu.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vgp.dianchejie.cn

================================================================================
来源：http://qer.yonumen.top

F. 文件与目录
来源：http://edb.guannengcc.top

================================================================================
来源：http://kdh.fehbvm.com

[F01] 读取整个文件
来源：http://ytp.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ewy.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://aow.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cpy.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oyw.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://trp.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sau.iojbl.cn

Ruby: File.read("a.txt")
来源：http://asm.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://dyl.dianchejie.cn

[F02] 逐行读取文件
来源：http://mjw.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vzj.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mjr.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cjo.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fzj.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wnu.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ryx.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ukm.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mvs.cheryme.top

[F03] 写入文件（覆盖）
来源：http://iaa.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aij.kuanghao11.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ter.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://klv.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kye.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xrc.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aks.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://xzd.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hhc.jyoumei.cn

[F04] 追加写入文件
来源：http://rxf.shanyushiyangtech.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wbg.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://htr.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xmf.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yoh.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ldl.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tbk.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gzo.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://waw.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://rzk.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xww.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://lin.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://yod.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://wvs.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://oui.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ijv.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://xqf.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://wsa.chenlongwang.top

[F06] 删除文件
来源：http://uhm.kuanghao11.cn

Py:   os.remove("a.txt")
来源：http://juk.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://rob.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://oej.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://mdy.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rgf.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://tmd.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://kcj.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://ksu.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://xov.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zof.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kdy.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://alc.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aor.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gwi.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vna.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yuo.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vfa.vqdsnc.cn

[F08] 遍历目录
来源：http://xba.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://icr.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xcl.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://lsa.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://lup.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tyz.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sut.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://fvz.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://vhl.zhijiandao.cn

[F09] 获取文件大小
来源：http://wsa.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://yxy.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://yfv.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://pce.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://kzy.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://alf.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://muz.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://ztw.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://zmb.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://kms.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bag.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lxx.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hwo.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://bdy.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cne.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ayg.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mgy.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wfw.jinqigufen.top

[F11] 复制与移动文件
来源：http://lxk.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yfn.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://psy.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hrf.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vry.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xbh.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tkn.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bgc.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zbp.hcnkem.com

[F12] CSV 读写
来源：http://gkt.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jbz.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jmn.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bsu.zhiwuduotai.top

TS:   // 同上
来源：http://thz.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nqk.jqgfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qlo.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cda.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ydv.yvedp.cn

================================================================================
来源：http://idm.guowangkeji.top

G. 面向对象
来源：http://qcy.jinqigfzy.top

================================================================================
来源：http://xyr.mhx1999.top

[G01] 定义类
来源：http://ybr.birdmap.top

Py:   class User: pass
来源：http://wyb.pengpengdd.cyou

PHP:  class User {}
来源：http://zbt.ywan-chungtsiang.top

JS:   class User {}
来源：http://iqp.cheryme.top

TS:   class User { name: string = ""; }
来源：http://kuw.gotoacloud.top


<!-- 参考信息 -->