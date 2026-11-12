代发 wailian999

C#:   s.Replace("a", "b")
来源：http://bck.mhx1999.top

[E07] 按分隔符拆分
来源：http://mii.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yvt.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tav.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://qzb.yongpay.top

TS:   s.split(",")
来源：http://ogd.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zag.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wal.yj202588.top

Ruby: s.split(",");  s.split
来源：http://ror.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vwd.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://xde.shuidangran.top

Py:   ",".join(items)
来源：http://tfh.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://brl.zhijiandao.cn

JS:   items.join(",")
来源：http://tks.fanxiaobao.xyz

TS:   items.join(",")
来源：http://yfa.ydzc1.top

Java: String.join(",", items)
来源：http://rnb.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://idx.hnxiangtu.top

Ruby: items.join(",")
来源：http://idq.zhixingplan.top

C#:   string.Join(",", items)
来源：http://xbf.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://swq.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zff.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rmv.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://drp.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://wbq.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://kjr.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jzc.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://qmh.yj20258.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cqz.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://bvz.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ezb.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hsr.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://ulp.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://qjg.shzxlz.cn

Java: String.format("%03d", 7)
来源：http://pdd.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uwz.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iih.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zek.chenlongwang.top

[E11] 反转字符串
来源：http://wsa.cdnleiting.top

Py:   s[::-1]
来源：http://arl.jianghu66.top

PHP:  strrev($s);
来源：http://jag.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://jmn.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://shh.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ryx.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nrq.hnxiangtu.top

Ruby: s.reverse
来源：http://ybk.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vxh.xinyue.icu

[E12] 统计某字符出现次数
来源：http://cid.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://yph.cqqwz.cn

PHP:  substr_count($s, "a");
来源：http://ofp.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://uwe.c1oappe.top

TS:   s.split("a").length - 1
来源：http://tyc.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tvh.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://dmp.sjlbkw.cn

Ruby: s.count("a")
来源：http://ksi.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://zie.chenlongwang.top

[E13] 逐字符遍历
来源：http://rqx.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://rgn.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xny.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wxr.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tjt.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vxa.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bfc.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qzl.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ccm.shanyushiyangtech.top

[E14] URL 编码与 Base64
来源：http://iou.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vto.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dts.fengsongda.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sih.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ajw.gotoacloud.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ivt.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lmm.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zwv.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wgu.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://hvm.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gzu.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://efd.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tfz.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ibt.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qkt.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rrs.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vkx.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wvw.yvedp.cn

[E16] 数字千分位
来源：http://tdj.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://wpu.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://gqw.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qmm.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rku.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xml.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wzf.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://prr.havefunace.top

C#:   1234567.ToString("N0")
来源：http://ekx.havefunace.top

[E17] 首字母大写
来源：http://czr.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oav.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qnb.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://peo.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ybs.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sqs.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lqj.cashguo.top

Ruby: s.capitalize
来源：http://cza.hfpthk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tpl.smart0.xyz

[E18] 模板占位符替换
来源：http://ksa.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qia.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ylb.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gmb.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://pch.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jlq.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tlt.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://itz.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://akm.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://afo.9152youxi.cn

Py:   s.splitlines()
来源：http://dyq.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qqn.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://ohh.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://zuc.ybcxt.top

Java: s.lines().toList()
来源：http://pfo.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://swb.tianlin.xyz

Ruby: s.lines
来源：http://uxy.redwolf501.top

C#:   s.Split('\n')
来源：http://yvx.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://rvu.meibo888.top

Py:   if not s:
来源：http://hrb.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ggz.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qmg.xuanzx.com

TS:   if (s === "") {}
来源：http://sqi.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://tdk.gotoacloud.top

Go:   if s == "" {}
来源：http://kyf.jqgfzy.top

Ruby: if s.empty?
来源：http://wns.zdqjudy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bqg.yj20258888.top

[E21] 超长截断加省略号
来源：http://owt.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://puz.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sdy.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynu.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://afk.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xwo.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://zjd.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xgy.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://adz.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://vuy.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ghp.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mgw.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wiv.nanxinkj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bce.svipenyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bog.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xcx.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://bwj.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jsy.yonumen.top

================================================================================
来源：http://dcq.fktsv.cn

F. 文件与目录
来源：http://mxy.yongpay.top

================================================================================
来源：http://pjt.yuxming.cn

[F01] 读取整个文件
来源：http://prh.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rus.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://fru.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qap.pengpengdd.cyou

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tvt.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ffs.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iih.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://cae.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://got.ehwqpu.com

[F02] 逐行读取文件
来源：http://mcq.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wrb.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bog.quarkkingdee.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vfb.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tzu.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://udz.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bml.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ahg.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bnn.sweek.top

[F03] 写入文件（覆盖）
来源：http://fmq.daxiang520.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zjv.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qxx.hysaishi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sjq.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mxd.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://njx.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wnh.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://gug.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oyw.kuanghao11.cn

[F04] 追加写入文件
来源：http://hff.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bcy.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://igo.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kzy.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wlr.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gud.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://swy.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cem.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rbu.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://lhj.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://svq.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://gcf.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://qxb.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://jlb.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kvd.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yzw.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://prk.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://ioi.hnqzz.top

[F06] 删除文件
来源：http://ncj.c1oappe.top

Py:   os.remove("a.txt")
来源：http://iiy.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://nzw.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lpm.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://aic.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yjt.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://ibx.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://fjq.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://wry.meibo888.top

[F07] 创建目录（含多级）
来源：http://kpz.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kal.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aip.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ngl.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pup.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xjp.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://npu.daria6918.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ror.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://huh.shangyingyoupin.top

[F08] 遍历目录
来源：http://dds.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wgx.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zrb.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://roi.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://rog.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mwj.yanxiufei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jlu.sufxvd.cn

Ruby: Dir.children("dir")
来源：http://ljl.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://scw.uphjek.com

[F09] 获取文件大小
来源：http://uze.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://nam.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://rcu.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://brr.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://xkg.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://sau.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tbi.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://uhz.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://xul.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://ftu.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wsp.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zeb.zycfv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bil.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://cmo.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://odn.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qxb.fehbvm.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dxo.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://asy.jqgufenzy.top

[F11] 复制与移动文件
来源：http://edu.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vqk.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uxb.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kcn.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pfq.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jsk.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oor.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sua.hesvh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sxd.fzhhl.top

[F12] CSV 读写
来源：http://sku.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mqv.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://smw.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xdn.wangdashe.top

TS:   // 同上
来源：http://xoy.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bqp.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wfk.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://riw.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://lgy.gaohongyu789.top

================================================================================
来源：http://upp.sxryk.cn

G. 面向对象
来源：http://chw.tarul.cn

================================================================================
来源：http://nkd.hesvh.cn

[G01] 定义类
来源：http://hqb.yuxming.cn

Py:   class User: pass
来源：http://iwb.chenzaomai.com

PHP:  class User {}
来源：http://vkh.zhongyouzk.top

JS:   class User {}
来源：http://hih.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://plf.redwolf501.top

Java: class User {}
来源：http://jmv.shuidangran.top

Go:   type User struct { Name string }
来源：http://ovl.wangshuangyany.cn

Ruby: class User; end
来源：http://xjc.xinyue.icu

C#:   class User {}
来源：http://oau.zhongyouzk.top

[G02] 构造函数
来源：http://mot.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ioo.wangdashe.top

PHP:  public function __construct(public string $name) {}
来源：http://fel.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://qez.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://wsu.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://nyu.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ift.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://ptf.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://rhk.52xcode.cn

[G03] 实例属性
来源：http://dfx.redwolf501.top

Py:   self.name = "x"
来源：http://uhw.ydzc1.top

PHP:  public string $name = "x";
来源：http://vjq.c1oappe.top

JS:   this.name = "x";
来源：http://fbe.yangfankeji.com

TS:   name: string = "x";
来源：http://lfi.dianchejie.cn

Java: private String name;
来源：http://mtq.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zrg.jqgufenzy.top

Ruby: @name = "x"
来源：http://mps.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://xlo.shuidangran.top

[G04] 定义方法
来源：http://eqs.hesvh.cn

Py:   def greet(self): return self.name
来源：http://lcu.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vzt.yuanzhike.top

JS:   greet() { return this.name; }
来源：http://est.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://mis.zhijiandao.cn

Java: String greet() { return name; }
来源：http://raz.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gku.jianghu66.top

Ruby: def greet; @name; end
来源：http://yao.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://rlb.guowangkeji.top

[G05] 继承
来源：http://hws.sweek.top

Py:   class Admin(User): pass
来源：http://zwr.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://hcy.meibo888.top

JS:   class Admin extends User {}
来源：http://gvl.fehbvm.com

TS:   class Admin extends User {}
来源：http://mnz.shanyushiyangkeji.top


<!-- 参考信息 -->