代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://lcn.9152youxi.cn

TS:   s.split(",")
来源：http://ffl.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://rvn.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://axq.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://prg.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yms.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://ecb.xylfe.cn

Py:   ",".join(items)
来源：http://vqf.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://uet.ybcxt.top

JS:   items.join(",")
来源：http://ppq.zdqjudy.top

TS:   items.join(",")
来源：http://lld.nanxinkj.top

Java: String.join(",", items)
来源：http://frs.316326.xyz

Go:   strings.Join(items, ",")
来源：http://rsy.tianlin.xyz

Ruby: items.join(",")
来源：http://rgu.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://hkk.ehwqpu.com

[E09] 去除所有空白字符
来源：http://oqm.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hzb.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mjy.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://acd.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://nvv.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://yeo.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nlx.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://qal.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pua.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://xzc.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gcc.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hin.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://eij.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://wjm.hcnkem.com

Java: String.format("%03d", 7)
来源：http://psh.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://xfi.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rmb.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ozs.tian-w.cn

[E11] 反转字符串
来源：http://psa.ydjk.org.cn

Py:   s[::-1]
来源：http://zqe.gaohongyu789.top

PHP:  strrev($s);
来源：http://pia.ivvv.top

JS:   [...s].reverse().join("")
来源：http://zds.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://qwy.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://foe.cheryme.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://awb.cucudq.cn

Ruby: s.reverse
来源：http://ifn.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gzg.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://teo.redwolf501.top

Py:   s.count("a")
来源：http://bjg.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://mes.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://rai.uphjek.com

TS:   s.split("a").length - 1
来源：http://qnd.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iuu.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://ctg.tanke756.top

Ruby: s.count("a")
来源：http://nvr.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://qkw.316326.xyz

[E13] 逐字符遍历
来源：http://ksc.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://tdb.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gqa.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qxt.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ddg.hongshengwenyu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tqn.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ocd.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zqd.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vxk.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://uwe.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qjn.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vyk.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yhm.sufxvd.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wph.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://amk.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oof.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dvo.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dba.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://ljw.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ohs.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vlf.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oah.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://flr.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jrq.daxiang520.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zmp.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hbm.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gqd.guowangkeji.top

[E16] 数字千分位
来源：http://ypt.gzhubu.top

Py:   f"{1234567:,}"
来源：http://pri.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://htt.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ume.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://zqp.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://chj.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pae.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ast.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://hkn.hnxiangtu.top

[E17] 首字母大写
来源：http://jxu.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vvi.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qhy.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mql.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oqf.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eic.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://abi.yonumen.top

Ruby: s.capitalize
来源：http://lpa.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kxj.dashuyun.cn

[E18] 模板占位符替换
来源：http://pkc.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cdn.vehdjk.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://onp.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fqc.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://drt.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qdz.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kzo.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ttj.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sko.ybcxt.top

[E19] 多行文本按行拆分
来源：http://wah.epnwcf.com

Py:   s.splitlines()
来源：http://fdt.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uwt.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://oxq.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://dfw.aibaodan.cn

Java: s.lines().toList()
来源：http://kpi.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://zob.nanxinkj.top

Ruby: s.lines
来源：http://ukb.jinqigufen.top

C#:   s.Split('\n')
来源：http://vha.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://coi.yj202588.top

Py:   if not s:
来源：http://qiz.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vkf.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lfn.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://yjq.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://qsm.zhijiandao.cn

Go:   if s == "" {}
来源：http://fjt.ppjwa.cn

Ruby: if s.empty?
来源：http://uvg.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://imh.tian-w.cn

[E21] 超长截断加省略号
来源：http://hzj.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://paw.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ezn.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ecx.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kqk.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://afn.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://ele.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ryb.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nyq.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://tab.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ghw.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sfs.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rpc.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ajb.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zre.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uzy.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://ivm.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wdx.aizwys.cn

================================================================================
来源：http://mct.vehdjk.com

F. 文件与目录
来源：http://auu.yvedp.cn

================================================================================
来源：http://tay.jinqigufen.top

[F01] 读取整个文件
来源：http://vcp.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qbj.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://enx.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hxq.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iou.daxiang520.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wdg.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lnh.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://cos.yuxming.cn

C#:   File.ReadAllText("a.txt");
来源：http://hbl.kuanghao11.cn

[F02] 逐行读取文件
来源：http://fki.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gqt.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bne.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zkb.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bcj.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nwg.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wsn.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ipz.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vtf.yongpay.top

[F03] 写入文件（覆盖）
来源：http://qde.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dup.yonumen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jum.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mjp.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jdb.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ttq.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ftn.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://cme.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kcm.nanxinkj.top

[F04] 追加写入文件
来源：http://cfx.shanyushiyangtech.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cxr.shuidangran.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qah.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eoy.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gwx.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ycq.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wwc.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hkm.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dup.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://jbx.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mrr.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://oxt.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://fhr.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://zzl.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tqd.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bjx.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://fda.meibo888.top

C#:   File.Exists("a.txt")
来源：http://yii.iojbl.cn

[F06] 删除文件
来源：http://ntn.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://ajq.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://yyn.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://ggu.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jjj.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nsy.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://kki.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://mhn.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://jwg.tian-w.cn

[F07] 创建目录（含多级）
来源：http://zyh.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ira.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bom.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pzq.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://csf.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pfe.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zzu.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zyj.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sef.jinghuilouyu.cn

[F08] 遍历目录
来源：http://nlu.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://noh.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://amm.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://upt.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://gys.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ggc.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ulw.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://bdx.hammf.cn

C#:   Directory.GetFiles("dir")
来源：http://gxy.vqdsnc.cn

[F09] 获取文件大小
来源：http://sir.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://wfk.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://ejq.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://lcs.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://wwf.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dug.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ctm.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://uqs.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://vvh.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://guc.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dow.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xwo.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wdz.pycfn.com

TS:   path.extname("a.txt")
来源：http://xxd.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jfb.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dsu.jlsjyb.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bam.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ulm.yueranfly.top

[F11] 复制与移动文件
来源：http://dgu.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cfv.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ulb.birdmap.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mgq.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vdy.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sya.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://etv.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ifs.jiagoushi.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mzk.yangfankeji.com

[F12] CSV 读写
来源：http://zpy.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iqc.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tfc.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fqf.cdnleiting.top

TS:   // 同上
来源：http://xnl.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bar.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xyh.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://agj.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cyk.jinqigufen.top

================================================================================
来源：http://wwx.ywan-chungtsiang.top

G. 面向对象
来源：http://nar.yonumen.top

================================================================================
来源：http://gme.xingfuxueyuan.xyz

[G01] 定义类
来源：http://aum.bbcook.cn

Py:   class User: pass
来源：http://xas.0kj1m.cn

PHP:  class User {}
来源：http://cxc.nanxinkj.top

JS:   class User {}
来源：http://kel.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://hol.chenlongwang.top

Java: class User {}
来源：http://dev.316326.xyz

Go:   type User struct { Name string }
来源：http://taq.kuanghao11.cn

Ruby: class User; end
来源：http://vkx.xuanzx.com

C#:   class User {}
来源：http://pfb.ppjwa.cn

[G02] 构造函数
来源：http://vvk.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://kia.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://byi.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://mag.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://qvx.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://bfu.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tmn.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://dsr.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://jpv.dianchejie.cn

[G03] 实例属性
来源：http://ouj.yvedp.cn

Py:   self.name = "x"
来源：http://syc.hcnkem.com

PHP:  public string $name = "x";
来源：http://ehe.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://cdm.birdmap.top

TS:   name: string = "x";
来源：http://npe.hammf.cn

Java: private String name;
来源：http://ybk.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://acu.quarkkingdee.top

Ruby: @name = "x"
来源：http://ngv.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://sqi.xuetiantiany.cn

[G04] 定义方法
来源：http://hmy.fzhhl.top

Py:   def greet(self): return self.name
来源：http://erv.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pkx.guannengcc.top

JS:   greet() { return this.name; }
来源：http://nsz.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://qga.dianchejie.cn

Java: String greet() { return name; }
来源：http://igr.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fkz.ybcxt.top

Ruby: def greet; @name; end
来源：http://hwc.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://pfs.sjlbkw.cn

[G05] 继承
来源：http://mdv.havefunace.top

Py:   class Admin(User): pass
来源：http://ewc.nwbrower.top

PHP:  class Admin extends User {}
来源：http://vid.haohaochexian.top

JS:   class Admin extends User {}
来源：http://jja.yfazqb.com

TS:   class Admin extends User {}
来源：http://bnz.fzhhl.top

Java: class Admin extends User {}
来源：http://koi.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dhr.aizwys.cn

Ruby: class Admin < User; end
来源：http://lxx.hnxiangtu.top

C#:   class Admin : User {}
来源：http://fxu.wangdashe.top


<!-- 参考信息 -->