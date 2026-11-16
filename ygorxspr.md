代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eou.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://arq.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rpb.chenjidiqi.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yhm.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ske.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yxt.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://jtm.jiagoushi.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rhp.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yne.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rmt.shuidangran.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qya.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ppq.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://abl.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rbv.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lrs.jiagoushi.top

[D26] 数组转字符串
来源：http://clx.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://wje.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://vis.hysaishi.cn

JS:   arr.join(", ")
来源：http://pbu.gogol.net.cn

TS:   arr.join(", ")
来源：http://uwa.9152youxi.cn

Java: String.join(", ", list)
来源：http://onq.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://chr.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://ytk.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://ejz.nanxuanxn.top

================================================================================
来源：http://xvs.jlsjyb.cn

E. 字符串处理
来源：http://aqg.shzxlz.cn

================================================================================
来源：http://acb.andypj.xyz

[E01] 拼接字符串
来源：http://rmo.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ujp.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lgt.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sju.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://saj.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ewc.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://flq.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eyd.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pnt.yanxiufei.cn

[E02] 重复字符串
来源：http://fir.yonumen.top

Py:   "ab" * 3
来源：http://hqp.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://ldz.iojbl.cn

JS:   "ab".repeat(3)
来源：http://bjw.fehbvm.com

TS:   "ab".repeat(3)
来源：http://set.hesvh.cn

Java: "ab".repeat(3)
来源：http://jkd.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://nyq.aizwys.cn

Ruby: "ab" * 3
来源：http://tst.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nhd.zdbjq.cn

[E03] 截取子串
来源：http://xbn.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://swg.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xjk.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ist.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://yfk.0kj1m.cn

Java: s.substring(1, 4)
来源：http://xcx.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tot.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://dmv.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://ypl.jyoumei.cn

[E04] 查找子串位置
来源：http://cnt.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://dtz.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://bnt.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://luy.jinqigufen.top

TS:   s.indexOf("x")
来源：http://gtv.zhijiandao.cn

Java: s.indexOf("x")
来源：http://dbb.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://lad.ctjpmb.com

Ruby: s.index("x")
来源：http://lgn.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://ths.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fzx.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jyy.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wpb.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tjj.yvedp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fvr.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kfj.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ymo.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sbj.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ypz.cheryme.top

[E06] 替换子串
来源：http://yxh.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ovu.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://omy.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xtx.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://gbr.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rjr.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ldv.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://buz.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://iaq.aizwys.cn

[E07] 按分隔符拆分
来源：http://eio.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ccr.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lnj.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vlz.yueranfly.top

TS:   s.split(",")
来源：http://zol.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://svj.xziqi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://svs.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://yqu.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ssb.xinyue.icu

[E08] 数组按分隔符合并
来源：http://fuy.ybcxt.top

Py:   ",".join(items)
来源：http://vsf.cheryme.top

PHP:  implode(",", $items);
来源：http://gvu.jqgufenzy.top

JS:   items.join(",")
来源：http://ysy.svipenyu.cn

TS:   items.join(",")
来源：http://zrp.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://fqw.pycfn.com

Go:   strings.Join(items, ",")
来源：http://nva.vqdsnc.cn

Ruby: items.join(",")
来源：http://pzr.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://bip.yj202588.top

[E09] 去除所有空白字符
来源：http://axj.ppjwa.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://deb.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ibd.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://wxq.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://hjm.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://bgo.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vpu.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://cgn.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://soz.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://bah.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ovt.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xhy.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://vqj.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://ruv.tian-w.cn

Java: String.format("%03d", 7)
来源：http://mou.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ldg.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mzi.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://euh.52xcode.cn

[E11] 反转字符串
来源：http://yer.tianlin.xyz

Py:   s[::-1]
来源：http://bcu.aizwys.cn

PHP:  strrev($s);
来源：http://vec.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://cfx.birdmap.top

TS:   [...s].reverse().join("")
来源：http://wqf.jyoumei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vni.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ber.zhiwuduotai.top

Ruby: s.reverse
来源：http://acm.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://loh.pycfn.com

[E12] 统计某字符出现次数
来源：http://ghk.hysaishi.cn

Py:   s.count("a")
来源：http://pzx.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://yty.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://hph.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://uuh.zdqjudy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wbq.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://pxt.hnqzz.top

Ruby: s.count("a")
来源：http://dwz.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://clx.guannengcc.top

[E13] 逐字符遍历
来源：http://ogo.tarul.cn

Py:   for ch in s: print(ch)
来源：http://tcn.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lvv.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nsz.jianghu66.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://egt.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fpy.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://flf.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sig.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blw.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://yak.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dcq.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ome.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xgt.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mjw.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pha.andypj.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cai.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://stg.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gwd.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://mjb.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tbi.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sgo.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zol.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://jnb.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qcp.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ppb.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ahg.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://poo.daxiang520.top

[E16] 数字千分位
来源：http://ivb.fzhhl.top

Py:   f"{1234567:,}"
来源：http://lrh.ehwqpu.com

PHP:  number_format(1234567);
来源：http://tbc.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qhp.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jhg.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hcv.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fdd.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://atw.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://thy.tarul.cn

[E17] 首字母大写
来源：http://qpi.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mdq.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yid.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mjo.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bsf.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pie.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tdn.shangyingyoupin.top

Ruby: s.capitalize
来源：http://ojs.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yhh.jinqigfzy.top

[E18] 模板占位符替换
来源：http://pxe.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mwi.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://byt.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ifj.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ugk.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xzz.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jiz.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xqu.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hmh.tian-w.cn

[E19] 多行文本按行拆分
来源：http://dxd.cdnleiting.top

Py:   s.splitlines()
来源：http://ijm.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://swd.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://wvf.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://kta.yueranfly.top

Java: s.lines().toList()
来源：http://myw.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://zbk.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://dhe.zycfv.cn

C#:   s.Split('\n')
来源：http://yvg.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://nwu.52xcode.cn

Py:   if not s:
来源：http://mos.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qgr.shuidangran.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vbh.tarul.cn

TS:   if (s === "") {}
来源：http://udv.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://wgi.yuxming.cn

Go:   if s == "" {}
来源：http://zap.hysaishi.cn

Ruby: if s.empty?
来源：http://wql.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zir.wangdashe.top

[E21] 超长截断加省略号
来源：http://otr.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zre.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cps.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bve.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sbt.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ehf.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://evk.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vys.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oxr.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://suv.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jav.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qyu.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ohj.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://snk.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aif.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hcr.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://vqu.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eah.yuanzhike.top

================================================================================
来源：http://cor.cqqwz.cn

F. 文件与目录
来源：http://wqk.havefunace.top

================================================================================
来源：http://puk.fehbvm.com

[F01] 读取整个文件
来源：http://wmg.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://apx.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://rkn.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hxm.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eqp.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gsz.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ako.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://qog.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://mch.zdbjq.cn

[F02] 逐行读取文件
来源：http://lwp.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ysx.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://elv.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wbn.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcy.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uor.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uca.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zko.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rhc.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://fak.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fwq.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xgz.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kju.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oda.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rch.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nca.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://evj.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fze.epnwcf.com

[F04] 追加写入文件
来源：http://ozh.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pva.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ggm.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lkd.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://umk.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://drn.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jez.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://set.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pyc.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://sqc.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ted.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://xgi.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://mvv.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://nhl.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ivk.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yzq.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://vjk.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://cbi.fktsv.cn

[F06] 删除文件
来源：http://hcu.shuidangran.top

Py:   os.remove("a.txt")
来源：http://ofz.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://lin.cashguo.top

JS:   fs.unlinkSync("a.txt")
来源：http://fae.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://aop.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qhk.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://qpr.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://rdv.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://svj.yj202588.top

[F07] 创建目录（含多级）
来源：http://ywn.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ofg.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uxf.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dnq.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ovz.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lzw.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xth.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vpv.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sfg.nanxuanxn.top

[F08] 遍历目录
来源：http://cxb.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://eku.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dmy.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://ekc.yueranfly.top

TS:   fs.readdirSync("dir")
来源：http://ojv.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fij.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zcr.uphjek.com

Ruby: Dir.children("dir")
来源：http://dhb.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://nwk.havefunace.top


<!-- 参考信息 -->