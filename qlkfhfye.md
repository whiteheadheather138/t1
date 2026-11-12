代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://lkg.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uwd.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tny.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pov.tarul.cn

C#:   s.Replace("a", "b")
来源：http://qge.hammf.cn

[E07] 按分隔符拆分
来源：http://zqc.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mpt.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eip.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tyd.epnwcf.com

TS:   s.split(",")
来源：http://uhl.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://bho.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vxx.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://grn.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rzp.sxryk.cn

[E08] 数组按分隔符合并
来源：http://dqw.jianghu66.top

Py:   ",".join(items)
来源：http://lmf.shuidangran.top

PHP:  implode(",", $items);
来源：http://wci.dianchejie.cn

JS:   items.join(",")
来源：http://fxz.cqqwz.cn

TS:   items.join(",")
来源：http://qxm.redwolf501.top

Java: String.join(",", items)
来源：http://vlh.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://gfm.jinqigufen.top

Ruby: items.join(",")
来源：http://wzk.tian-w.cn

C#:   string.Join(",", items)
来源：http://sys.yuxming.cn

[E09] 去除所有空白字符
来源：http://jfk.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eiv.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://emq.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://tnt.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://lzi.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://acc.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fvd.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://ktd.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://acm.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://aea.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ahk.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tqe.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://ckb.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://qlm.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://zvd.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://gpc.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rxw.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bot.dianchejie.cn

[E11] 反转字符串
来源：http://kap.aibaodan.cn

Py:   s[::-1]
来源：http://dcd.tianlin.xyz

PHP:  strrev($s);
来源：http://zpf.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://fgy.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://bfo.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://dhl.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uvx.tanke756.top

Ruby: s.reverse
来源：http://dzn.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jcn.yongpay.top

[E12] 统计某字符出现次数
来源：http://kvm.bjfxy.top

Py:   s.count("a")
来源：http://dee.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://qut.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://qlp.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://mkd.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gvs.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://kps.haohaochexian.top

Ruby: s.count("a")
来源：http://ogt.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://dif.cashguo.top

[E13] 逐字符遍历
来源：http://ckj.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://rdr.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vtl.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ony.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cpl.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bva.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iwg.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://cul.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yjb.xziqi.cn

[E14] URL 编码与 Base64
来源：http://pqh.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qfz.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://usp.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dxp.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rpq.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jht.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iku.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bak.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mak.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://mrh.jyoumei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sov.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://epf.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uvn.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://crd.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qxe.ydzc1.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ldb.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hnc.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ygj.svipenyu.cn

[E16] 数字千分位
来源：http://hwd.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://cgz.chenzaomai.com

PHP:  number_format(1234567);
来源：http://ttq.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nmp.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://moe.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zdk.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tws.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oum.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://njh.birdmap.top

[E17] 首字母大写
来源：http://noi.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://esa.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://emm.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://avd.mhx1999.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ibx.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uxu.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sas.tian-w.cn

Ruby: s.capitalize
来源：http://xij.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nnu.fzhhl.top

[E18] 模板占位符替换
来源：http://ats.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kda.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jwt.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://hgt.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jgo.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yjx.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://djc.guannengcc.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xhe.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ilq.sysykeji.top

[E19] 多行文本按行拆分
来源：http://nga.hesvh.cn

Py:   s.splitlines()
来源：http://uos.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wkl.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://vdv.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://wpa.yfazqb.com

Java: s.lines().toList()
来源：http://jps.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://wwg.gotoacloud.top

Ruby: s.lines
来源：http://tup.jianghu66.top

C#:   s.Split('\n')
来源：http://ctv.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://cjs.andypj.xyz

Py:   if not s:
来源：http://mfj.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zmz.shangyingyoupin.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ech.aizwys.cn

TS:   if (s === "") {}
来源：http://zoz.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://qls.daria6918.cn

Go:   if s == "" {}
来源：http://uzg.nanxuanxn.top

Ruby: if s.empty?
来源：http://vla.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ceq.c1oappe.top

[E21] 超长截断加省略号
来源：http://kcy.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qvc.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vbf.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jmg.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://llv.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wxh.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://xaw.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://roe.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lll.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://dqu.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://naa.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ovu.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ofe.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyu.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ygs.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zbf.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://tpu.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://guc.chenlongwang.top

================================================================================
来源：http://zev.chenjidiqi.icu

F. 文件与目录
来源：http://meb.zhengqikj.top

================================================================================
来源：http://fmo.aibaodan.cn

[F01] 读取整个文件
来源：http://tct.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://plw.gotoacloud.top

PHP:  file_get_contents("a.txt");
来源：http://ysz.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mdg.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://deb.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://czr.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://elz.xziqi.cn

Ruby: File.read("a.txt")
来源：http://bge.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://qph.vehdjk.com

[F02] 逐行读取文件
来源：http://mnt.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://urx.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oht.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iop.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://afw.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hnu.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kfn.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://obi.zhixingplan.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fpk.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://cwa.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vgc.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://cmb.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ksm.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxq.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cgb.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bol.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://nqf.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oze.sjlbkw.cn

[F04] 追加写入文件
来源：http://fvs.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zhy.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nmg.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hzq.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ghx.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tun.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qcq.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fwe.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tky.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://vzt.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dpq.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://rbv.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://ydz.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://yfv.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://krb.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cvj.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://jjs.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://cpb.zhengqikj.top

[F06] 删除文件
来源：http://vdm.xylfe.cn

Py:   os.remove("a.txt")
来源：http://ahk.daxiang520.top

PHP:  unlink("a.txt");
来源：http://fro.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://uor.ydjk.org.cn

TS:   fs.unlinkSync("a.txt")
来源：http://enr.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://grm.uphjek.com

Go:   os.Remove("a.txt")
来源：http://uzc.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://tum.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://nye.hammf.cn

[F07] 创建目录（含多级）
来源：http://seu.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xrg.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vid.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kot.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mvo.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vyn.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://djk.ybcxt.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tmz.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://skz.yvedp.cn

[F08] 遍历目录
来源：http://crp.vqdsnc.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zzn.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://emp.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://iai.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://lhv.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nhu.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wjk.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://gdf.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://djl.chenjidiqi.icu

[F09] 获取文件大小
来源：http://lgf.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://mdh.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://hzh.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://hog.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://cvd.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://eix.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aar.xuanzx.com

Ruby: File.size("a.txt")
来源：http://kmx.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://typ.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://asi.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bkw.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dto.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pso.uphjek.com

TS:   path.extname("a.txt")
来源：http://xdd.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rkm.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gwv.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uzu.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ihx.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://sqf.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://flo.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iiq.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vnv.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nbv.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kvg.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://isp.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rcy.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vyn.nanxuanxn.top

[F12] CSV 读写
来源：http://cbb.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iqc.xinyue.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ytv.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cge.pycfn.com

TS:   // 同上
来源：http://tpg.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://typ.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aac.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://czf.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://ebd.nwbrower.top

================================================================================
来源：http://gep.cashguo.top

G. 面向对象
来源：http://kuc.xinyue.icu

================================================================================
来源：http://xdd.hywenlv.cn

[G01] 定义类
来源：http://cbv.zhoulong.xyz

Py:   class User: pass
来源：http://qte.shanyushiyangkeji.top

PHP:  class User {}
来源：http://aog.meibo888.top

JS:   class User {}
来源：http://gow.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://qkz.iojbl.cn

Java: class User {}
来源：http://jlw.iojbl.cn

Go:   type User struct { Name string }
来源：http://nal.dashuyun.cn

Ruby: class User; end
来源：http://fhk.andypj.xyz

C#:   class User {}
来源：http://hma.hnxiangtu.top

[G02] 构造函数
来源：http://aur.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://eug.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://zqg.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://uyx.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://tjy.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://nlt.yongpay.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wut.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://wfk.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://ojw.cucudq.cn

[G03] 实例属性
来源：http://jsj.xziqi.cn

Py:   self.name = "x"
来源：http://jrz.gotoacloud.top

PHP:  public string $name = "x";
来源：http://uwb.jinqigufen.top

JS:   this.name = "x";
来源：http://vgb.svipenyu.cn

TS:   name: string = "x";
来源：http://tdh.tianlin.xyz

Java: private String name;
来源：http://ixm.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vbd.hesvh.cn

Ruby: @name = "x"
来源：http://ybl.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://eca.zhiwuduotai.top

[G04] 定义方法
来源：http://ouz.yongpay.top

Py:   def greet(self): return self.name
来源：http://baq.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qkh.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://mdc.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://cmb.jinqigufen.top

Java: String greet() { return name; }
来源：http://itl.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://wmt.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://kyj.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://omv.jinqigufen.top

[G05] 继承
来源：http://jnw.ydjk.org.cn


<!-- 参考信息 -->