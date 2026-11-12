代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gpm.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://myf.svipenyu.cn

Go:   // 手写循环
来源：http://kzn.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ohb.jianghu66.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nlz.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://hqk.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://egx.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zaj.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ptn.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kxx.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://swo.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lxk.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gsd.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tyh.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://vxj.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qem.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xyt.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sya.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fwr.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://koe.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hgi.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qfn.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lwq.wangdashe.top

[D26] 数组转字符串
来源：http://cys.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://wvs.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://bah.jlsjyb.cn

JS:   arr.join(", ")
来源：http://uya.havefunace.top

TS:   arr.join(", ")
来源：http://cxc.cqqwz.cn

Java: String.join(", ", list)
来源：http://lne.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://zhx.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://knh.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://shk.xinyue.icu

================================================================================
来源：http://tnw.birdmap.top

E. 字符串处理
来源：http://fjj.gotoacloud.top

================================================================================
来源：http://dcv.zycfv.cn

[E01] 拼接字符串
来源：http://bzi.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ymb.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://avh.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mtb.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yqd.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zhj.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kea.iojbl.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://txi.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bkd.guowangkeji.top

[E02] 重复字符串
来源：http://xqt.ybcxt.top

Py:   "ab" * 3
来源：http://kug.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://qpb.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://jhk.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://aee.fengsongda.top

Java: "ab".repeat(3)
来源：http://dxg.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://dle.hcnkem.com

Ruby: "ab" * 3
来源：http://bbq.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mcw.ehwqpu.com

[E03] 截取子串
来源：http://coe.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nvm.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xhq.nanxuanxn.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sdr.shuidangran.top

TS:   s.slice(1, 4)
来源：http://lhk.zhixingplan.top

Java: s.substring(1, 4)
来源：http://ssu.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jrz.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://ngn.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://tvz.tarul.cn

[E04] 查找子串位置
来源：http://bst.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://gfp.daria6918.cn

PHP:  strpos($s, "x");
来源：http://cjk.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pdr.nwbrower.top

TS:   s.indexOf("x")
来源：http://krs.birdmap.top

Java: s.indexOf("x")
来源：http://tes.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://jau.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://kcv.316326.xyz

C#:   s.IndexOf("x")
来源：http://pbb.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pgm.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qaf.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yoa.xinyue.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vld.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eel.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wyu.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://inz.guannengcc.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kuw.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rmm.hnxiangtu.top

[E06] 替换子串
来源：http://pml.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oln.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://nym.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qho.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://rqt.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gfs.xziqi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ghr.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qnn.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://orc.zdbjq.cn

[E07] 按分隔符拆分
来源：http://xvw.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://siz.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vxq.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://icj.c1oappe.top

TS:   s.split(",")
来源：http://spy.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ugg.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://afs.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://vza.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xvs.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://oth.redwolf501.top

Py:   ",".join(items)
来源：http://pkn.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://aai.zhengqikj.top

JS:   items.join(",")
来源：http://pko.iojbl.cn

TS:   items.join(",")
来源：http://axd.jinqigfzy.top

Java: String.join(",", items)
来源：http://nwk.ivvv.top

Go:   strings.Join(items, ",")
来源：http://yuk.jqgufenzy.top

Ruby: items.join(",")
来源：http://iar.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://ivz.hywenlv.cn

[E09] 去除所有空白字符
来源：http://css.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vgq.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ujn.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://rpz.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://gdn.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://kcz.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rcc.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://rxe.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qmk.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://lpa.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rlj.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ief.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://lpx.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://gbx.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://owk.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bky.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pec.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hta.aizwys.cn

[E11] 反转字符串
来源：http://sbb.epnwcf.com

Py:   s[::-1]
来源：http://iqz.havefunace.top

PHP:  strrev($s);
来源：http://vgk.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://hji.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://qeq.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://amr.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dts.yvedp.cn

Ruby: s.reverse
来源：http://zlx.cashguo.top

C#:   new string(s.Reverse().ToArray())
来源：http://wtk.xziqi.cn

[E12] 统计某字符出现次数
来源：http://jtw.zhixingplan.top

Py:   s.count("a")
来源：http://gsb.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://osf.wangdashe.top

JS:   s.split("a").length - 1
来源：http://klz.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://qci.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zvt.ppjwa.cn

Go:   strings.Count(s, "a")
来源：http://ksh.ydjk.org.cn

Ruby: s.count("a")
来源：http://nyk.vehdjk.com

C#:   s.Count(c => c == 'a')
来源：http://knh.wangdashe.top

[E13] 逐字符遍历
来源：http://ame.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://fwi.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dym.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://btk.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://eml.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dzz.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yhz.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qyx.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zee.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://srm.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rxx.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://tgg.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ogs.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uzm.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ktm.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pcc.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vjl.sjlbkw.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pad.shanyushiyangkeji.top

[E15] HTML 转义 / 反转义
来源：http://mvg.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ncp.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aud.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iki.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xqq.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xmh.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ajy.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ewu.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://znx.cashguo.top

[E16] 数字千分位
来源：http://mex.chenlongwang.top

Py:   f"{1234567:,}"
来源：http://rkq.yvedp.cn

PHP:  number_format(1234567);
来源：http://mht.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://izt.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://owx.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iji.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yth.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lov.316326.xyz

C#:   1234567.ToString("N0")
来源：http://cqi.hammf.cn

[E17] 首字母大写
来源：http://vnt.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dty.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qkj.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lrc.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aqh.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bgj.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wde.zycfv.cn

Ruby: s.capitalize
来源：http://scz.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qdr.yj20258888.top

[E18] 模板占位符替换
来源：http://ery.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fra.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hmv.chenzaomai.com

JS:   tpl.replaceAll("{name}", name)
来源：http://lfa.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ilw.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://inl.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dmk.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zie.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tey.hnqzz.top

[E19] 多行文本按行拆分
来源：http://bhg.gogol.net.cn

Py:   s.splitlines()
来源：http://yhv.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hma.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://xrb.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://rgu.andypj.xyz

Java: s.lines().toList()
来源：http://ubx.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://ibv.gaohongyu789.top

Ruby: s.lines
来源：http://vay.hcnkem.com

C#:   s.Split('\n')
来源：http://kuv.yj20258888.top

[E20] 判断字符串是否为空
来源：http://uir.ybcxt.top

Py:   if not s:
来源：http://mtd.andypj.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yuy.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://asx.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://rkp.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://rbn.iojbl.cn

Go:   if s == "" {}
来源：http://tim.zycfv.cn

Ruby: if s.empty?
来源：http://bcp.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bgo.meibo888.top

[E21] 超长截断加省略号
来源：http://osi.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mzl.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zqg.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sez.bbcook.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lun.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uso.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://xfi.ydjk.org.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sdk.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nim.shzxlz.cn

[E22] 字节长度与字符长度
来源：http://dmf.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jgn.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yoh.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hfi.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ioe.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ppr.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://thc.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://tty.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://maw.fanxiaobao.xyz

================================================================================
来源：http://pgs.sweek.top

F. 文件与目录
来源：http://pls.chenjidiqi.icu

================================================================================
来源：http://rri.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://qww.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mje.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://zdd.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ofj.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uxi.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nkd.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mqm.bbcook.cn

Ruby: File.read("a.txt")
来源：http://ozw.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://ezi.ydjk.org.cn

[F02] 逐行读取文件
来源：http://tsm.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uql.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mkd.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ihg.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tvx.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://byp.zycfv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ute.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gie.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qpu.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://bfo.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ucj.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://inr.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://scy.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxm.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hhk.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jyq.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://awv.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://alk.jqgfzy.top

[F04] 追加写入文件
来源：http://eio.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tip.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yio.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://joo.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rwj.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yrm.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cqv.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wvw.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dkt.jqgufenzy.top

[F05] 判断文件或目录是否存在
来源：http://yfa.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ewc.sweek.top

PHP:  file_exists("a.txt");
来源：http://eqv.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://prh.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://dok.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://syl.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nug.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://ooo.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://hxl.havefunace.top

[F06] 删除文件
来源：http://yun.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://trp.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://dgl.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://zia.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://joj.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tdv.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://tbn.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://gxp.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://igd.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://dci.yj202588.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jlj.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yqt.ywan-chungtsiang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bpo.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://akp.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://czb.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qfy.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oyp.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cai.zdqjudy.top

[F08] 遍历目录
来源：http://mhp.yj20258888.top


<!-- 参考信息 -->