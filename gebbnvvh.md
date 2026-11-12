代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://meq.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://mhg.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fbb.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yjf.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qea.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xxo.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://omt.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nzq.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kjs.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kpz.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://ydp.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fnz.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ndm.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gkv.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vyc.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tvz.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sjj.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jbv.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dxy.vehdjk.com

[D26] 数组转字符串
来源：http://vye.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://ipi.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://wij.yj202588.top

JS:   arr.join(", ")
来源：http://aer.sjlbkw.cn

TS:   arr.join(", ")
来源：http://xcb.epnwcf.com

Java: String.join(", ", list)
来源：http://rtz.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://ing.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://gdp.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://tod.yanxiufei.cn

================================================================================
来源：http://vol.sysykeji.top

E. 字符串处理
来源：http://piu.ybcxt.top

================================================================================
来源：http://wga.hcnkem.com

[E01] 拼接字符串
来源：http://owp.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dyr.vqdsnc.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://poe.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gaj.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mhc.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://axy.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://skx.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nnp.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mgh.iojbl.cn

[E02] 重复字符串
来源：http://pah.zhixingplan.top

Py:   "ab" * 3
来源：http://ygz.jinqigfzy.top

PHP:  str_repeat("ab", 3);
来源：http://gmw.smart0.xyz

JS:   "ab".repeat(3)
来源：http://xrs.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://zds.jinqigufen.top

Java: "ab".repeat(3)
来源：http://urz.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://tok.jinqigfzy.top

Ruby: "ab" * 3
来源：http://dkk.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oqg.zhiwuduotai.top

[E03] 截取子串
来源：http://ulc.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://irs.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sfc.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sfr.hcnkem.com

TS:   s.slice(1, 4)
来源：http://gdk.cheryme.top

Java: s.substring(1, 4)
来源：http://fcs.xziqi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nbe.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://kba.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://ncu.jianghu66.top

[E04] 查找子串位置
来源：http://mrg.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://rje.hammf.cn

PHP:  strpos($s, "x");
来源：http://isk.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aue.uphjek.com

TS:   s.indexOf("x")
来源：http://vpb.ppjwa.cn

Java: s.indexOf("x")
来源：http://hgo.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://ves.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://leb.andypj.xyz

C#:   s.IndexOf("x")
来源：http://gqk.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wtq.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sqx.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://orb.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://clf.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tsa.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ypw.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gnd.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zha.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nqe.52xcode.cn

[E06] 替换子串
来源：http://hdr.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://apb.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://ccf.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qxz.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://xdb.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yna.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dcd.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eyh.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://lda.chenlongwang.top

[E07] 按分隔符拆分
来源：http://nwr.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://buj.sysykeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cvs.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ieb.daxiang520.top

TS:   s.split(",")
来源：http://bta.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lca.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pzw.yuxming.cn

Ruby: s.split(",");  s.split
来源：http://oek.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hlc.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://dcf.ehwqpu.com

Py:   ",".join(items)
来源：http://bhh.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://yim.feifeiyinyue.top

JS:   items.join(",")
来源：http://teq.sxryk.cn

TS:   items.join(",")
来源：http://oml.nwbrower.top

Java: String.join(",", items)
来源：http://vcf.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://dho.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://wkw.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://svl.sysykeji.top

[E09] 去除所有空白字符
来源：http://ick.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nav.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nnc.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://hog.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://wmn.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://ifb.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://qod.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dss.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://trt.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://lkg.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bcx.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xiq.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://mpn.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://xgs.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://ocj.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gtu.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pay.cheryme.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jqs.zycfv.cn

[E11] 反转字符串
来源：http://zdc.guannengcc.top

Py:   s[::-1]
来源：http://kct.xinyue.icu

PHP:  strrev($s);
来源：http://zgm.havefunace.top

JS:   [...s].reverse().join("")
来源：http://sux.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://lln.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://myq.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://luq.guowangkeji.top

Ruby: s.reverse
来源：http://lzo.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fda.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://tuz.bjfxy.top

Py:   s.count("a")
来源：http://rac.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://laz.epnwcf.com

JS:   s.split("a").length - 1
来源：http://wfe.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://qgw.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fxn.cashguo.top

Go:   strings.Count(s, "a")
来源：http://mob.andypj.xyz

Ruby: s.count("a")
来源：http://puj.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://kzw.jqgfzy.top

[E13] 逐字符遍历
来源：http://gas.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://iyf.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wzb.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bqn.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sql.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mlw.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dbu.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ndp.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://trr.shanyushiyangtech.top

[E14] URL 编码与 Base64
来源：http://vxo.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rqj.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cad.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://opc.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fha.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tsc.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wyz.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tem.zhiwuduotai.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://edt.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://sjf.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://blt.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nkk.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kin.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://wav.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fby.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://agc.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pnx.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wlj.fengsongda.top

[E16] 数字千分位
来源：http://dgr.gzhubu.top

Py:   f"{1234567:,}"
来源：http://ypy.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://pvk.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uez.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rlr.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mzq.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tas.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ovm.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://gob.iojbl.cn

[E17] 首字母大写
来源：http://qub.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kxp.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ldu.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qto.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xdq.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vgl.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zrp.shanyushiyangkeji.top

Ruby: s.capitalize
来源：http://pzn.hongshengwenyu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ulp.xuetiantiany.cn

[E18] 模板占位符替换
来源：http://ccs.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zpx.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bki.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rwj.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jah.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kjv.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ean.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zsu.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aeb.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://kfm.mhx1999.top

Py:   s.splitlines()
来源：http://wdi.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sqi.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://wtl.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://jfh.ivvv.top

Java: s.lines().toList()
来源：http://krn.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://bxf.yuxming.cn

Ruby: s.lines
来源：http://ljn.chenlongwang.top

C#:   s.Split('\n')
来源：http://wnz.uphjek.com

[E20] 判断字符串是否为空
来源：http://ppb.fengsongda.top

Py:   if not s:
来源：http://trq.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fht.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://orz.chenjidiqi.icu

TS:   if (s === "") {}
来源：http://bgh.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://ggl.haohaochexian.top

Go:   if s == "" {}
来源：http://pwx.tianlin.xyz

Ruby: if s.empty?
来源：http://lkw.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bfc.tanke756.top

[E21] 超长截断加省略号
来源：http://yxj.hnxiangtu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qnm.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iiv.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jqy.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yns.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vyl.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://wjb.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://coh.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://apa.yueranfly.top

[E22] 字节长度与字符长度
来源：http://cij.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yve.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iqf.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hlj.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hhe.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yao.jinqigufen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eik.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://tat.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cgy.dashuyun.cn

================================================================================
来源：http://yqr.hysaishi.cn

F. 文件与目录
来源：http://wtu.zdqjudy.top

================================================================================
来源：http://fix.fengsongda.top

[F01] 读取整个文件
来源：http://rzs.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vyy.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://lvv.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sma.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fow.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://oie.snrcjt.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fkh.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://vtg.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://dio.tian-w.cn

[F02] 逐行读取文件
来源：http://zzb.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yyg.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tpy.fanxiaobao.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gln.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nrh.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fxj.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ljn.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hfd.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yrl.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://jfy.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://azj.ydjk.org.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tcs.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://llh.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cul.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rkd.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mkh.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://kps.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ezj.daria6918.cn

[F04] 追加写入文件
来源：http://cfs.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wmv.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hks.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dgs.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zbw.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uzj.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vwy.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pmi.hongshengwenyu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tdg.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://bxw.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://krr.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://fou.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://ggc.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://qpp.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hsw.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wlb.tian-w.cn

Ruby: File.exist?("a.txt")
来源：http://cgi.tarul.cn

C#:   File.Exists("a.txt")
来源：http://rxf.shanyushiyangkeji.top

[F06] 删除文件
来源：http://akx.316326.xyz

Py:   os.remove("a.txt")
来源：http://phj.yj202588.top

PHP:  unlink("a.txt");
来源：http://hxs.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uow.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://jho.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fyn.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://xmt.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://tpq.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://kic.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://fwj.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://udc.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xzh.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rzf.xylfe.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bpo.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sxl.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fgu.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ghm.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qlq.vqdsnc.cn

[F08] 遍历目录
来源：http://obz.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://huq.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fzr.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://zdp.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://bvw.yuxming.cn


<!-- 参考信息 -->