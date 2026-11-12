代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://upe.sysykeji.top

Ruby: arr.include?(x)
来源：http://fam.chenzaomai.com

C#:   list.Contains(x)
来源：http://qxb.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://ctz.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://icc.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://awi.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lxa.sufxvd.cn

TS:   [...arr];
来源：http://tac.meibo888.top

Java: new ArrayList<>(list);
来源：http://gct.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dil.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://znx.vqdsnc.cn

C#:   new List<int>(list);
来源：http://wuk.vqdsnc.cn

[D23] reduce 累积计算
来源：http://jss.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tgx.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qhk.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://utn.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rky.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ulc.jinqigfzy.top

Go:   // 手写循环
来源：http://voi.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oeu.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nvm.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://fff.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ofs.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vam.tanke756.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iio.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fse.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ena.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fow.andypj.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dxp.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qyq.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://ovt.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xce.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://flo.bjfxy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wmz.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://snc.zhaomingkeji.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ngv.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ygc.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mja.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dbi.yonumen.top

[D26] 数组转字符串
来源：http://dep.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://eyf.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://yzi.epnwcf.com

JS:   arr.join(", ")
来源：http://rrn.dianchejie.cn

TS:   arr.join(", ")
来源：http://uyw.snrcjt.cn

Java: String.join(", ", list)
来源：http://ejw.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://dsa.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://idf.sysykeji.top

C#:   string.Join(", ", list)
来源：http://mfy.jinqigfzy.top

================================================================================
来源：http://wfr.redwolf501.top

E. 字符串处理
来源：http://jrh.nwbrower.top

================================================================================
来源：http://nul.hongshengwenyu.top

[E01] 拼接字符串
来源：http://wfq.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://llh.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://udb.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gqo.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yif.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jlf.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qtk.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iuw.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rxk.andypj.xyz

[E02] 重复字符串
来源：http://pwe.shzxlz.cn

Py:   "ab" * 3
来源：http://pva.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://lvt.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://zgu.yj20258.top

TS:   "ab".repeat(3)
来源：http://fzg.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://sdh.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://kjt.yfazqb.com

Ruby: "ab" * 3
来源：http://jxp.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oyb.hnxiangtu.top

[E03] 截取子串
来源：http://pnn.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eew.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bve.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wbp.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://zvd.jiagoushi.top

Java: s.substring(1, 4)
来源：http://ttx.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lsb.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://djx.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://kto.cqqwz.cn

[E04] 查找子串位置
来源：http://edh.nanxinkj.top

Py:   s.find("x");  s.index("x")
来源：http://ium.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://ope.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tiy.havefunace.top

TS:   s.indexOf("x")
来源：http://ocm.kuanghao11.cn

Java: s.indexOf("x")
来源：http://rbx.zhaomingkeji.xyz

Go:   strings.Index(s, "x")
来源：http://hyt.feifeiyinyue.top

Ruby: s.index("x")
来源：http://ucn.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://ayo.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xev.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jvb.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tbp.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wbi.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://osy.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://adj.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yyw.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oyl.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dhp.tanke756.top

[E06] 替换子串
来源：http://zpj.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pyx.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://oea.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tnr.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://olz.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kon.bbcook.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yyz.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://chn.tanke756.top

C#:   s.Replace("a", "b")
来源：http://yqt.yangfankeji.com

[E07] 按分隔符拆分
来源：http://ksz.xuetiantiany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mfr.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jol.yuxming.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yrw.fktsv.cn

TS:   s.split(",")
来源：http://rfa.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nsx.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qaw.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://ddb.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sjb.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://zdg.yanxiufei.cn

Py:   ",".join(items)
来源：http://cmj.shuidangran.top

PHP:  implode(",", $items);
来源：http://aiv.jianghu66.top

JS:   items.join(",")
来源：http://lvi.yj20258.top

TS:   items.join(",")
来源：http://ofd.zhengqikj.top

Java: String.join(",", items)
来源：http://qvd.chenlongwang.top

Go:   strings.Join(items, ",")
来源：http://usa.jiagoushi.top

Ruby: items.join(",")
来源：http://ama.zhengqikj.top

C#:   string.Join(",", items)
来源：http://bpm.chenzaomai.com

[E09] 去除所有空白字符
来源：http://rlj.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bkv.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wcs.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://eab.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://kzd.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://kta.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fsg.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oaf.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pgv.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://ygr.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bha.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://axf.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://wdb.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://btd.zycfv.cn

Java: String.format("%03d", 7)
来源：http://npv.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bkn.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wys.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rkk.xziqi.cn

[E11] 反转字符串
来源：http://iqt.yvedp.cn

Py:   s[::-1]
来源：http://mbd.yj202588.top

PHP:  strrev($s);
来源：http://cso.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://whz.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://hzi.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://wwl.sjlbkw.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pge.ppjwa.cn

Ruby: s.reverse
来源：http://fvh.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://hzf.yj202588.top

[E12] 统计某字符出现次数
来源：http://kxu.fanxiaobao.xyz

Py:   s.count("a")
来源：http://uiu.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://vob.tarul.cn

JS:   s.split("a").length - 1
来源：http://qnt.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://zfj.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jpy.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://qlb.sweek.top

Ruby: s.count("a")
来源：http://wsf.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://pbd.sweek.top

[E13] 逐字符遍历
来源：http://pzt.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://uoi.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mwf.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://div.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pda.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ujd.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zwf.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://joe.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xli.havefunace.top

[E14] URL 编码与 Base64
来源：http://mib.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ncg.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://wzn.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fgl.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sso.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kjm.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zrw.iojbl.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rok.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://atk.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://lbl.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ogi.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pxz.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dhd.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aai.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hpx.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pgw.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iie.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://egn.zhongyouzk.top

[E16] 数字千分位
来源：http://tve.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://zln.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://gbh.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kzj.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rey.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rgm.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sfn.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yaw.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://rwi.52xcode.cn

[E17] 首字母大写
来源：http://wpu.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ncw.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hty.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oqf.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wqs.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://stf.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xkz.snrcjt.cn

Ruby: s.capitalize
来源：http://aks.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://squ.hesvh.cn

[E18] 模板占位符替换
来源：http://nwq.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iim.vehdjk.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iev.jinqigfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zos.jinqigufen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://myb.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rpw.ehwqpu.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://utw.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iiu.sysykeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rss.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://dhl.tianlin.xyz

Py:   s.splitlines()
来源：http://zoj.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mnh.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://gkz.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://qsi.iojbl.cn

Java: s.lines().toList()
来源：http://ogd.dianchejie.cn

Go:   strings.Split(s, "\n")
来源：http://ekn.gaohongyu789.top

Ruby: s.lines
来源：http://vie.aizwys.cn

C#:   s.Split('\n')
来源：http://jxl.zhijiandao.cn

[E20] 判断字符串是否为空
来源：http://vhi.sxryk.cn

Py:   if not s:
来源：http://asp.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tvq.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://arj.xuanzx.com

TS:   if (s === "") {}
来源：http://aix.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://wtq.nanxuanxn.top

Go:   if s == "" {}
来源：http://jkf.nwbrower.top

Ruby: if s.empty?
来源：http://mxf.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wdi.daxiang520.top

[E21] 超长截断加省略号
来源：http://xne.dianchejie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vcw.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://klc.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xok.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nub.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://squ.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://ptn.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tze.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://afv.hesvh.cn

[E22] 字节长度与字符长度
来源：http://rgf.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gvq.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yjc.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://klz.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eap.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://otz.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kbu.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://xnu.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jiz.sysykeji.top

================================================================================
来源：http://inv.cucudq.cn

F. 文件与目录
来源：http://kcl.nwbrower.top

================================================================================
来源：http://oau.sufxvd.cn

[F01] 读取整个文件
来源：http://wkl.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pse.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://lrj.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mfx.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://irz.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hzy.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mhf.yongpay.top

Ruby: File.read("a.txt")
来源：http://djd.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://vzj.ivvv.top

[F02] 逐行读取文件
来源：http://fyg.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vte.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nyo.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://odh.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dzo.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://crc.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqh.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wnf.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://akz.uphjek.com

[F03] 写入文件（覆盖）
来源：http://aae.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lxc.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://vgx.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dde.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ocz.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jye.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://syb.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://hxy.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jlu.shzxlz.cn

[F04] 追加写入文件
来源：http://drs.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zub.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://syh.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wog.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://guq.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fsn.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://use.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ykj.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sxl.hammf.cn

[F05] 判断文件或目录是否存在
来源：http://zfz.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://syb.meibo888.top

PHP:  file_exists("a.txt");
来源：http://qzd.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://kac.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://xef.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kpf.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mjj.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://ndp.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://ten.ppjwa.cn

[F06] 删除文件
来源：http://qlr.ivvv.top

Py:   os.remove("a.txt")
来源：http://thg.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://gay.nanxinkj.top


<!-- 参考信息 -->