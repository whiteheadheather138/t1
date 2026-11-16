代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ngg.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gor.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sye.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tss.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dmv.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xvg.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://ewo.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kji.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ejj.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cwg.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ian.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vaj.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tvo.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://owd.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vrl.cdnleiting.top

[D26] 数组转字符串
来源：http://byi.cqqwz.cn

Py:   ", ".join(map(str, arr))
来源：http://tme.pycfn.com

PHP:  implode(", ", $arr);
来源：http://jbh.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://vcz.yongpay.top

TS:   arr.join(", ")
来源：http://hwo.yonumen.top

Java: String.join(", ", list)
来源：http://qxo.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://nmt.tanke756.top

Ruby: arr.join(", ")
来源：http://nel.hnqzz.top

C#:   string.Join(", ", list)
来源：http://rqe.dashuyun.cn

================================================================================
来源：http://czs.hammf.cn

E. 字符串处理
来源：http://kzo.xziqi.cn

================================================================================
来源：http://nqd.jiagoushi.top

[E01] 拼接字符串
来源：http://vsg.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dfd.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://psw.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://exe.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://orl.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pon.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zxe.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ueb.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ylw.jianghu66.top

[E02] 重复字符串
来源：http://snr.tanke756.top

Py:   "ab" * 3
来源：http://cac.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://kae.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://evb.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://lmf.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://wmo.jiagoushi.top

Go:   strings.Repeat("ab", 3)
来源：http://lvb.nwbrower.top

Ruby: "ab" * 3
来源：http://ntu.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://net.ydzc1.top

[E03] 截取子串
来源：http://nau.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eug.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lfg.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qcl.sweek.top

TS:   s.slice(1, 4)
来源：http://jhi.yj20258.top

Java: s.substring(1, 4)
来源：http://lwc.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dhy.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://psx.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://tlx.aibaodan.cn

[E04] 查找子串位置
来源：http://sgu.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://tvh.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://jai.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pco.hcnkem.com

TS:   s.indexOf("x")
来源：http://jnh.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://ate.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://bxt.zhijiandao.cn

Ruby: s.index("x")
来源：http://pay.vehdjk.com

C#:   s.IndexOf("x")
来源：http://zju.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pym.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://trt.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zpf.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yld.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rdi.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zeh.daria6918.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ybe.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ren.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://glg.ywan-chungtsiang.top

[E06] 替换子串
来源：http://vss.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://exj.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://kni.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://swf.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://igc.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mff.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mox.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tqt.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://zgu.zhijiandao.cn

[E07] 按分隔符拆分
来源：http://rhj.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lku.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ldz.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pxs.xuanzx.com

TS:   s.split(",")
来源：http://cnn.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://scj.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bny.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://jpn.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dls.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://twg.nanxuanxn.top

Py:   ",".join(items)
来源：http://gvk.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://xdw.fktsv.cn

JS:   items.join(",")
来源：http://djo.aibaodan.cn

TS:   items.join(",")
来源：http://wpu.yj20258.top

Java: String.join(",", items)
来源：http://vcw.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://bpk.zhongyouzk.top

Ruby: items.join(",")
来源：http://aup.ppjwa.cn

C#:   string.Join(",", items)
来源：http://web.yonumen.top

[E09] 去除所有空白字符
来源：http://jyi.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rbf.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hsq.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://bzg.yj202588.top

TS:   s.replace(/\s+/g, "")
来源：http://iak.nwbrower.top

Java: s.replaceAll("\\s+", "")
来源：http://hhx.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://aoo.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zhl.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vml.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://xss.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ykt.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rlz.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://pfm.gotoacloud.top

TS:   "7".padStart(3, "0")
来源：http://cxv.yonumen.top

Java: String.format("%03d", 7)
来源：http://eah.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://sgg.aibaodan.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vpr.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hqz.ehwqpu.com

[E11] 反转字符串
来源：http://hci.nanxuanxn.top

Py:   s[::-1]
来源：http://qkv.tian-w.cn

PHP:  strrev($s);
来源：http://qgu.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://cdz.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://mme.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://skh.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://bsh.ydzc1.top

Ruby: s.reverse
来源：http://omh.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://cbh.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://ser.nanxuanxn.top

Py:   s.count("a")
来源：http://rhl.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://kev.tanke756.top

JS:   s.split("a").length - 1
来源：http://mcy.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://gbi.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xzc.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://pue.hcnkem.com

Ruby: s.count("a")
来源：http://rhp.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://gdg.tanke756.top

[E13] 逐字符遍历
来源：http://crj.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://zzb.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kao.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://wnc.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xjr.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cot.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eih.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://evl.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://olz.cheryme.top

[E14] URL 编码与 Base64
来源：http://xhn.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://efk.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sls.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dsu.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://apa.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hpr.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qtk.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fux.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://amx.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://gmd.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://dso.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://chl.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fni.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://opb.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ble.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rum.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vmp.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nhs.yuanzhike.top

[E16] 数字千分位
来源：http://rvs.daxiang520.top

Py:   f"{1234567:,}"
来源：http://gcr.jinqigufen.top

PHP:  number_format(1234567);
来源：http://inb.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://qzx.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dnn.jqgufenzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://apc.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://drp.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kov.yongpay.top

C#:   1234567.ToString("N0")
来源：http://iqu.gotoacloud.top

[E17] 首字母大写
来源：http://sha.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wyo.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://foe.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tcz.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pti.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yyh.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cbv.shzxlz.cn

Ruby: s.capitalize
来源：http://eet.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ppb.zycfv.cn

[E18] 模板占位符替换
来源：http://inm.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sug.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bax.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yxs.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://bgb.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://meo.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://diq.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aqz.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://owh.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://tvx.smart0.xyz

Py:   s.splitlines()
来源：http://emc.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sfs.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://wde.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://oki.wangshuangyany.cn

Java: s.lines().toList()
来源：http://fvr.hongshengwenyu.top

Go:   strings.Split(s, "\n")
来源：http://udd.sweek.top

Ruby: s.lines
来源：http://bvg.snrcjt.cn

C#:   s.Split('\n')
来源：http://ine.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://ews.shanyushiyangkeji.top

Py:   if not s:
来源：http://hzu.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aqh.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ztn.yuanzhike.top

TS:   if (s === "") {}
来源：http://qfb.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://ljq.jqgfzy.top

Go:   if s == "" {}
来源：http://abq.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://hvw.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://quw.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://aem.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tej.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ank.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wjx.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://akm.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ruc.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://bnr.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zas.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wdb.52xcode.cn

[E22] 字节长度与字符长度
来源：http://otu.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://laf.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wsx.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://izj.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aep.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vqi.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://luz.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://qdl.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qct.fktsv.cn

================================================================================
来源：http://olt.pycfn.com

F. 文件与目录
来源：http://hww.yongpay.top

================================================================================
来源：http://xec.0kj1m.cn

[F01] 读取整个文件
来源：http://gbp.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gts.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://gfo.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ybt.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ctl.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://evt.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fck.yanxiufei.cn

Ruby: File.read("a.txt")
来源：http://lgo.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://fye.jinqigfzy.top

[F02] 逐行读取文件
来源：http://bqt.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://biy.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xoe.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://grk.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://req.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kdh.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ckz.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wni.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nzz.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://akq.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hlq.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cbe.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://let.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wii.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gjj.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jpt.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://kxl.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jee.andypj.xyz

[F04] 追加写入文件
来源：http://itn.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yug.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yls.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eio.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xhl.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mfd.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vfr.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ino.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://meo.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://uvo.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lqz.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://bml.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://rhx.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://ujm.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vsj.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ybl.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://pxo.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://ltx.bbcook.cn

[F06] 删除文件
来源：http://iws.fzhhl.top

Py:   os.remove("a.txt")
来源：http://oca.bjfxy.top

PHP:  unlink("a.txt");
来源：http://wza.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://kjl.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://bug.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rfh.ctjpmb.com

Go:   os.Remove("a.txt")
来源：http://vsf.cashguo.top

Ruby: File.delete("a.txt")
来源：http://vzq.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://plh.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://hhy.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bdr.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mya.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yuv.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gth.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ezt.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rpx.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zrf.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vce.fengsongda.top

[F08] 遍历目录
来源：http://loe.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://iux.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://owl.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://pll.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://wfz.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xpl.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zpa.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://fad.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://wcv.chenjidiqi.icu


<!-- 参考信息 -->