代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nfj.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://wdo.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ynh.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nzk.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://txg.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zac.mhx1999.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fjf.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://khe.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://poy.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ceg.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://ymw.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eft.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qle.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bqm.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kwc.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wrh.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nnb.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fvy.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://viz.sweek.top

[D26] 数组转字符串
来源：http://evk.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://dml.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://ktb.aizwys.cn

JS:   arr.join(", ")
来源：http://gsc.cdnleiting.top

TS:   arr.join(", ")
来源：http://jnw.shzxlz.cn

Java: String.join(", ", list)
来源：http://ndb.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://lpp.zhengqikj.top

Ruby: arr.join(", ")
来源：http://mpt.nwbrower.top

C#:   string.Join(", ", list)
来源：http://wvg.jqgfzy.top

================================================================================
来源：http://jng.daria6918.cn

E. 字符串处理
来源：http://kuo.ivvv.top

================================================================================
来源：http://rkm.bbcook.cn

[E01] 拼接字符串
来源：http://sry.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xsi.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zao.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jvo.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yhz.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nln.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wji.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hgn.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fmx.yueranfly.top

[E02] 重复字符串
来源：http://nxv.chenlongwang.top

Py:   "ab" * 3
来源：http://lqd.vqdsnc.cn

PHP:  str_repeat("ab", 3);
来源：http://teg.fzhhl.top

JS:   "ab".repeat(3)
来源：http://wwy.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://qsy.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://fgh.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://thq.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://cfl.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kaq.aizwys.cn

[E03] 截取子串
来源：http://ceo.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aaw.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yri.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jkz.havefunace.top

TS:   s.slice(1, 4)
来源：http://nqw.hcnkem.com

Java: s.substring(1, 4)
来源：http://vyy.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hpk.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ikd.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://gbd.meibo888.top

[E04] 查找子串位置
来源：http://dgp.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://ezq.yj202588.top

PHP:  strpos($s, "x");
来源：http://ytg.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iyr.ehwqpu.com

TS:   s.indexOf("x")
来源：http://uva.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://gri.yonumen.top

Go:   strings.Index(s, "x")
来源：http://vii.yj202588.top

Ruby: s.index("x")
来源：http://aef.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://rru.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vqc.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://myc.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hus.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cun.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kbr.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kks.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eqt.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zyt.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sfa.guowangkeji.top

[E06] 替换子串
来源：http://lhj.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hiq.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://zls.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ztn.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://kfo.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qwm.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kro.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://imz.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://hju.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://wpi.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bkt.sjlbkw.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mlx.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iey.guannengcc.top

TS:   s.split(",")
来源：http://dur.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://iap.vqdsnc.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aug.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://muz.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ini.ivvv.top

[E08] 数组按分隔符合并
来源：http://qqs.feifeiyinyue.top

Py:   ",".join(items)
来源：http://pnb.yangfankeji.com

PHP:  implode(",", $items);
来源：http://ejx.cqqwz.cn

JS:   items.join(",")
来源：http://nrm.birdmap.top

TS:   items.join(",")
来源：http://qau.jqgfzy.top

Java: String.join(",", items)
来源：http://hlc.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://hvk.ydzc1.top

Ruby: items.join(",")
来源：http://yzy.haohaochexian.top

C#:   string.Join(",", items)
来源：http://bll.zycfv.cn

[E09] 去除所有空白字符
来源：http://rgm.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://atj.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ele.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://msg.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://zoh.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://ptz.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://idy.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://tkx.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kce.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://nmg.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gxj.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tgj.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://qkl.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://smk.yonumen.top

Java: String.format("%03d", 7)
来源：http://cft.bbcook.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://emp.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gpp.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hkh.yj20258888.top

[E11] 反转字符串
来源：http://slg.52xcode.cn

Py:   s[::-1]
来源：http://ugi.zhengqikj.top

PHP:  strrev($s);
来源：http://kjc.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://awt.sweek.top

TS:   [...s].reverse().join("")
来源：http://abe.zhaomingkeji.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ria.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jgn.yangfankeji.com

Ruby: s.reverse
来源：http://kco.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://aff.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://cvg.9152youxi.cn

Py:   s.count("a")
来源：http://gkn.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://sra.mhx1999.top

JS:   s.split("a").length - 1
来源：http://nzi.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://ksu.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aoq.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://pnr.ctjpmb.com

Ruby: s.count("a")
来源：http://kzn.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://bsr.jqgfzy.top

[E13] 逐字符遍历
来源：http://mer.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://btx.yongpay.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ydd.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xai.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oco.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iee.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pjz.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ddn.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wgd.shanyushiyangkeji.top

[E14] URL 编码与 Base64
来源：http://vol.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aev.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ftq.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cct.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://saj.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zpm.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ocd.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iue.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vxv.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://skd.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mmr.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fil.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://knj.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wmn.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kme.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bmi.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://afz.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uda.iojbl.cn

[E16] 数字千分位
来源：http://yjs.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://cyr.0kj1m.cn

PHP:  number_format(1234567);
来源：http://lkl.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hni.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rte.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qmd.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://khy.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mgj.316326.xyz

C#:   1234567.ToString("N0")
来源：http://iau.xinyue.icu

[E17] 首字母大写
来源：http://ote.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kdy.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mbs.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wle.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jyz.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ksp.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cbj.jlsjyb.cn

Ruby: s.capitalize
来源：http://tyu.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uum.daxiang520.top

[E18] 模板占位符替换
来源：http://wjp.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jut.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bmr.yj20258.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gnd.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lvp.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lhs.guannengcc.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bgx.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jwn.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kjg.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://qrk.cdnleiting.top

Py:   s.splitlines()
来源：http://ekf.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nww.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://xvv.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://xcs.ehwqpu.com

Java: s.lines().toList()
来源：http://fih.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://scw.tian-w.cn

Ruby: s.lines
来源：http://abe.ehwqpu.com

C#:   s.Split('\n')
来源：http://xbo.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://qwy.hcnkem.com

Py:   if not s:
来源：http://poi.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mfa.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://stx.aibaodan.cn

TS:   if (s === "") {}
来源：http://xuv.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://lba.nwbrower.top

Go:   if s == "" {}
来源：http://nqp.redwolf501.top

Ruby: if s.empty?
来源：http://vge.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nrt.haohaochexian.top

[E21] 超长截断加省略号
来源：http://xiu.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nkd.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eys.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jtv.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sul.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oub.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://mft.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wkp.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gnd.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://qld.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://utv.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bro.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ede.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tex.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jig.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dbr.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://bwv.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uxy.shanyushiyangtech.top

================================================================================
来源：http://hjw.sufxvd.cn

F. 文件与目录
来源：http://ryo.dashuyun.cn

================================================================================
来源：http://aul.yuanzhike.top

[F01] 读取整个文件
来源：http://srj.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ffc.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://jvy.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bqk.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://slq.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://azd.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aka.jianghu66.top

Ruby: File.read("a.txt")
来源：http://osv.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://zbc.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://uzx.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fwo.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qei.iojbl.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hdg.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qcs.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://knq.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tqa.yvedp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cic.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vjh.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://zou.ehwqpu.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ahk.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oyb.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://voo.snrcjt.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mwx.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nls.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xzu.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://ddw.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kye.tarul.cn

[F04] 追加写入文件
来源：http://eps.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wdt.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nmk.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gfc.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ugi.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lfn.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sjc.xinyue.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rai.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yui.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://ijq.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://khw.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://cyw.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://dry.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://kpr.yvedp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aim.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wcz.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://blz.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://scw.zdbjq.cn

[F06] 删除文件
来源：http://elh.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://wpy.smart0.xyz

PHP:  unlink("a.txt");
来源：http://hot.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://iqp.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tzy.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dvk.yonumen.top

Go:   os.Remove("a.txt")
来源：http://umj.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://snq.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://orw.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://xkb.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dje.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pcv.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://olc.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kuz.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kft.dashuyun.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jmy.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nbq.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jyo.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://msq.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rpy.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xto.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://ngg.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://uab.fktsv.cn


<!-- 参考信息 -->