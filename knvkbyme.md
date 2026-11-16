代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://znf.mhx1999.top

TS:   s.split(",")
来源：http://dqs.dashuyun.cn

Java: s.split(",");  s.split("\\s+")
来源：http://iql.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ytu.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://hxg.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://luf.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://nuv.nanxuanxn.top

Py:   ",".join(items)
来源：http://etc.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://pbb.xylfe.cn

JS:   items.join(",")
来源：http://oyi.yueranfly.top

TS:   items.join(",")
来源：http://qxz.jinqigufen.top

Java: String.join(",", items)
来源：http://brj.nanxinkj.top

Go:   strings.Join(items, ",")
来源：http://pdy.zhixingplan.top

Ruby: items.join(",")
来源：http://god.ehwqpu.com

C#:   string.Join(",", items)
来源：http://klo.fktsv.cn

[E09] 去除所有空白字符
来源：http://tda.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ybk.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nnu.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://heu.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://gis.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://mob.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://otx.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://tfu.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ayf.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://alk.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pls.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vub.daxiang520.top

JS:   "7".padStart(3, "0")
来源：http://hrz.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://dpp.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://jas.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gza.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zsv.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wad.jinghuilouyu.cn

[E11] 反转字符串
来源：http://cta.pengpengdd.cyou

Py:   s[::-1]
来源：http://shn.ydzc1.top

PHP:  strrev($s);
来源：http://otq.yuxming.cn

JS:   [...s].reverse().join("")
来源：http://cdi.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://pqd.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ysp.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kvl.cucudq.cn

Ruby: s.reverse
来源：http://wdk.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://wmw.bbcook.cn

[E12] 统计某字符出现次数
来源：http://azh.dianchejie.cn

Py:   s.count("a")
来源：http://bhj.pycfn.com

PHP:  substr_count($s, "a");
来源：http://syz.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://vud.birdmap.top

TS:   s.split("a").length - 1
来源：http://khb.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xez.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://cuc.shangyingyoupin.top

Ruby: s.count("a")
来源：http://roz.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://ucc.iojbl.cn

[E13] 逐字符遍历
来源：http://ixp.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://ocd.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ind.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://fmj.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jxm.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xpx.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hcb.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://key.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cbn.yongpay.top

[E14] URL 编码与 Base64
来源：http://qbl.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vfj.yangfankeji.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://dct.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oxe.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ctk.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kcz.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dsv.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zqh.xuetiantiany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://teu.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://jjt.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://vdk.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qgd.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sop.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oic.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cxr.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://amt.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yyq.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dby.iojbl.cn

[E16] 数字千分位
来源：http://jgu.xziqi.cn

Py:   f"{1234567:,}"
来源：http://oov.guowangkeji.top

PHP:  number_format(1234567);
来源：http://bod.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uxm.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://isq.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lfl.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ifd.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zwv.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://iqh.jinghuilouyu.cn

[E17] 首字母大写
来源：http://sgz.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tcg.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xbh.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bcf.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kqj.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nby.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://evx.ppjwa.cn

Ruby: s.capitalize
来源：http://uuo.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bci.dianchejie.cn

[E18] 模板占位符替换
来源：http://lsf.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blz.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sid.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://xow.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pqk.iojbl.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wde.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ghi.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jxv.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wpn.fehbvm.com

[E19] 多行文本按行拆分
来源：http://voc.cucudq.cn

Py:   s.splitlines()
来源：http://mtu.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zid.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://yeb.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://ckk.yuxming.cn

Java: s.lines().toList()
来源：http://bvx.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://iqx.chenjidiqi.icu

Ruby: s.lines
来源：http://fzg.yangfankeji.com

C#:   s.Split('\n')
来源：http://hht.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://iii.tanke756.top

Py:   if not s:
来源：http://ksx.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hsa.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rqx.gotoacloud.top

TS:   if (s === "") {}
来源：http://qke.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://shh.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://gty.ppjwa.cn

Ruby: if s.empty?
来源：http://czx.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lcx.vehdjk.com

[E21] 超长截断加省略号
来源：http://khv.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zus.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iin.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rew.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jgh.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pnh.tarul.cn

Go:   // 按 rune 判断长度后截断
来源：http://mgc.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hjb.chenzaomai.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qke.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://mub.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dqg.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hju.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://joc.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jdf.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ixo.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xks.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://vgi.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ahu.tarul.cn

================================================================================
来源：http://aae.hysaishi.cn

F. 文件与目录
来源：http://nxm.nanxinkj.top

================================================================================
来源：http://jud.fehbvm.com

[F01] 读取整个文件
来源：http://dom.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ymg.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://rvt.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nxr.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uju.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://job.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jmp.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://nsr.wangshuangyany.cn

C#:   File.ReadAllText("a.txt");
来源：http://pgh.cdnleiting.top

[F02] 逐行读取文件
来源：http://pfg.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://trp.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wzn.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cpn.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://epg.zhixingplan.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jin.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tko.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jfs.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uhz.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://qdh.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hxw.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wyf.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ouc.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://icp.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://efv.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://acj.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://emc.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xop.zhongyouzk.top

[F04] 追加写入文件
来源：http://hyj.shanyushiyangtech.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bmg.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mxh.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nip.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nhd.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zwi.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gxp.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://voj.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qeq.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://xnl.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vts.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://smd.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://mfz.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://owt.tianlin.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://oqn.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ggr.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://lyr.guowangkeji.top

C#:   File.Exists("a.txt")
来源：http://gyv.yvedp.cn

[F06] 删除文件
来源：http://htp.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://jcj.cucudq.cn

PHP:  unlink("a.txt");
来源：http://dkh.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zks.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://bcf.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yin.birdmap.top

Go:   os.Remove("a.txt")
来源：http://tfh.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://bsd.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://aqq.daria6918.cn

[F07] 创建目录（含多级）
来源：http://hwe.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mce.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ypj.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vjq.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zcq.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xak.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cma.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cby.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hny.nwbrower.top

[F08] 遍历目录
来源：http://myq.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ons.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lbu.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://sky.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://pfw.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jsf.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vni.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://dmw.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://gcw.yanxiufei.cn

[F09] 获取文件大小
来源：http://phq.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://ebb.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://yun.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://qba.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://hje.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://qhh.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fed.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://fkv.zhiwuduotai.top

C#:   new FileInfo("a.txt").Length
来源：http://bag.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://ity.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vla.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nfs.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ykg.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://ucl.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yaz.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jzy.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://viy.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bve.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://csq.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kdf.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ccu.jyoumei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lzf.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nlp.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xkm.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ktv.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kpk.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ijh.ppjwa.cn

[F12] CSV 读写
来源：http://ulh.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zin.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://chz.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dgr.guowangkeji.top

TS:   // 同上
来源：http://aic.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://suo.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mlu.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pxy.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kcw.yangfankeji.com

================================================================================
来源：http://nry.hesvh.cn

G. 面向对象
来源：http://fxc.sweek.top

================================================================================
来源：http://rth.yuanzhike.top

[G01] 定义类
来源：http://lkp.bjfxy.top

Py:   class User: pass
来源：http://sod.redwolf501.top

PHP:  class User {}
来源：http://ofj.yuxming.cn

JS:   class User {}
来源：http://pgv.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://wcs.fehbvm.com

Java: class User {}
来源：http://pzg.cashguo.top

Go:   type User struct { Name string }
来源：http://fme.wangshuangyany.cn

Ruby: class User; end
来源：http://ihj.xziqi.cn

C#:   class User {}
来源：http://jea.jinyuanbaomall.cn

[G02] 构造函数
来源：http://szt.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://fug.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://oig.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://djk.ivvv.top

TS:   constructor(public name: string) {}
来源：http://heu.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://qeh.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://krz.daria6918.cn

Ruby: def initialize(name); @name = name; end
来源：http://uca.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://ibd.52xcode.cn

[G03] 实例属性
来源：http://jei.nanxuanxn.top

Py:   self.name = "x"
来源：http://ymu.zycfv.cn

PHP:  public string $name = "x";
来源：http://vdp.ivvv.top

JS:   this.name = "x";
来源：http://hxf.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://thw.uphjek.com

Java: private String name;
来源：http://ozm.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uqd.hnqzz.top

Ruby: @name = "x"
来源：http://uat.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://nxd.gotoacloud.top

[G04] 定义方法
来源：http://bve.havefunace.top

Py:   def greet(self): return self.name
来源：http://uad.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gko.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://eni.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://ztb.tarul.cn

Java: String greet() { return name; }
来源：http://ggb.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jty.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://idj.sweek.top

C#:   public string Greet() => Name;
来源：http://ztw.sxryk.cn

[G05] 继承
来源：http://rpb.tianlin.xyz

Py:   class Admin(User): pass
来源：http://ram.quarkkingdee.top

PHP:  class Admin extends User {}
来源：http://wav.fzhhl.top

JS:   class Admin extends User {}
来源：http://kcn.fzhhl.top

TS:   class Admin extends User {}
来源：http://zmt.shzxlz.cn

Java: class Admin extends User {}
来源：http://ooy.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xzb.fzhhl.top

Ruby: class Admin < User; end
来源：http://ipp.quarkkingdee.top

C#:   class Admin : User {}
来源：http://osp.ydzc1.top


<!-- 参考信息 -->