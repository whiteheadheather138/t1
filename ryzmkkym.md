代发 wailian999

Ruby: arr.tally
来源：http://yrx.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://teq.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://qtg.ydjk.org.cn

Py:   x in arr
来源：http://tns.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://jwp.ppjwa.cn

JS:   arr.includes(x)
来源：http://bxw.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://uxj.hfpthk.cn

Java: list.contains(x)
来源：http://ibq.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://rib.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://yoz.birdmap.top

C#:   list.Contains(x)
来源：http://vwp.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://btr.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ycp.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vel.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dwe.jlsjyb.cn

TS:   [...arr];
来源：http://htn.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://znb.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://spp.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://whs.gaohongyu789.top

C#:   new List<int>(list);
来源：http://ndd.daria6918.cn

[D23] reduce 累积计算
来源：http://uyh.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xhd.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lny.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qrk.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jvr.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kqr.yj20258.top

Go:   // 手写循环
来源：http://pfe.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gae.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fkl.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://tdt.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://odu.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mpm.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xlp.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yyk.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ryk.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xvg.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ejg.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ucl.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://hnf.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fgd.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yzi.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xwc.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ggw.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://csp.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kwx.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rfi.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cvi.epnwcf.com

[D26] 数组转字符串
来源：http://vxt.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://gbv.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://dvy.jinqigfzy.top

JS:   arr.join(", ")
来源：http://axx.cucudq.cn

TS:   arr.join(", ")
来源：http://opp.bbcook.cn

Java: String.join(", ", list)
来源：http://lfs.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://hey.hnqzz.top

Ruby: arr.join(", ")
来源：http://vid.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://tfp.kuanghao11.cn

================================================================================
来源：http://gsr.xuanzx.com

E. 字符串处理
来源：http://wsn.sxryk.cn

================================================================================
来源：http://kgi.hammf.cn

[E01] 拼接字符串
来源：http://lls.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zrq.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fhp.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nyp.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wam.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://brd.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fip.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wxn.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://myu.tianlin.xyz

[E02] 重复字符串
来源：http://osy.zhixingplan.top

Py:   "ab" * 3
来源：http://kyv.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://dun.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://ack.xuanzx.com

TS:   "ab".repeat(3)
来源：http://fjw.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://ckp.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://sba.dashuyun.cn

Ruby: "ab" * 3
来源：http://nfc.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tym.ydzc1.top

[E03] 截取子串
来源：http://lxl.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zxq.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kyb.316326.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fdg.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://jxw.cdnleiting.top

Java: s.substring(1, 4)
来源：http://qmm.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hsw.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://qob.birdmap.top

C#:   s.Substring(1, 3)
来源：http://rti.gaohongyu789.top

[E04] 查找子串位置
来源：http://qsz.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://jvi.uphjek.com

PHP:  strpos($s, "x");
来源：http://ghx.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://naa.jqgfzy.top

TS:   s.indexOf("x")
来源：http://hlo.jqgfzy.top

Java: s.indexOf("x")
来源：http://qof.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://gqb.yj20258.top

Ruby: s.index("x")
来源：http://kov.bbcook.cn

C#:   s.IndexOf("x")
来源：http://kye.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://udo.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jzq.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oqb.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://swb.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lbf.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ubv.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gxy.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fth.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://alw.cqqwz.cn

[E06] 替换子串
来源：http://opd.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dcr.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://anf.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ufq.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://qcf.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kpz.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wjq.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gzo.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://pfo.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://dwp.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qtt.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tih.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://adh.hongshengwenyu.top

TS:   s.split(",")
来源：http://ycj.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://pxy.xziqi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://skc.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://bqi.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://azt.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://vxh.jianghu66.top

Py:   ",".join(items)
来源：http://wsu.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://cdj.gaohongyu789.top

JS:   items.join(",")
来源：http://uuj.jinghuilouyu.cn

TS:   items.join(",")
来源：http://rbk.jinqigufen.top

Java: String.join(",", items)
来源：http://dqj.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://kne.sufxvd.cn

Ruby: items.join(",")
来源：http://thz.jiagoushi.top

C#:   string.Join(",", items)
来源：http://bxl.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://zcj.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nle.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qwi.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://cmt.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://baj.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://jwt.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ehe.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://awg.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://grc.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://nof.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://llj.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gtx.zhongyouzk.top

JS:   "7".padStart(3, "0")
来源：http://yik.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://pdx.ppjwa.cn

Java: String.format("%03d", 7)
来源：http://dgy.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://npq.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://asv.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aca.meibo888.top

[E11] 反转字符串
来源：http://mwb.jyoumei.cn

Py:   s[::-1]
来源：http://wyq.mhx1999.top

PHP:  strrev($s);
来源：http://ptw.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://qre.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://xaw.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jid.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bgc.hammf.cn

Ruby: s.reverse
来源：http://qlh.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ddg.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://osz.aizwys.cn

Py:   s.count("a")
来源：http://utf.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://opz.meibo888.top

JS:   s.split("a").length - 1
来源：http://gdh.xylfe.cn

TS:   s.split("a").length - 1
来源：http://cxu.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bws.shanyushiyangkeji.top

Go:   strings.Count(s, "a")
来源：http://vki.zdqjudy.top

Ruby: s.count("a")
来源：http://pmh.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://zss.zdbjq.cn

[E13] 逐字符遍历
来源：http://nik.daxiang520.top

Py:   for ch in s: print(ch)
来源：http://ola.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nus.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sjk.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fuf.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pii.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oyk.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hje.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fpy.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://try.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://utp.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yfp.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hxy.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rxu.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dga.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kpr.guowangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wwn.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uwd.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://gdz.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hbt.guannengcc.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://emt.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ten.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tgf.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://evf.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://edt.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nuc.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://exg.yanxiufei.cn

[E16] 数字千分位
来源：http://pur.xylfe.cn

Py:   f"{1234567:,}"
来源：http://jxu.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://wps.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tqg.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rjg.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pxn.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qtj.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dfm.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://vbr.hesvh.cn

[E17] 首字母大写
来源：http://fef.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pkf.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://umi.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wwy.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ehx.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bix.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://izn.snrcjt.cn

Ruby: s.capitalize
来源：http://mts.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yah.zycfv.cn

[E18] 模板占位符替换
来源：http://afs.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://okp.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tpg.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ubq.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://poy.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hzj.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dju.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ldt.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wdk.wangdashe.top

[E19] 多行文本按行拆分
来源：http://cvj.chenzaomai.com

Py:   s.splitlines()
来源：http://dxh.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ilj.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://hlf.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://epy.xuanzx.com

Java: s.lines().toList()
来源：http://kah.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://ekq.zhaomingkeji.xyz

Ruby: s.lines
来源：http://enp.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://pfu.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://kem.yanxiufei.cn

Py:   if not s:
来源：http://gqw.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xto.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bmh.kuanghao11.cn

TS:   if (s === "") {}
来源：http://rev.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://czi.smart0.xyz

Go:   if s == "" {}
来源：http://xpy.jinqigfzy.top

Ruby: if s.empty?
来源：http://tqn.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gzv.xuanzx.com

[E21] 超长截断加省略号
来源：http://uyi.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tbe.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://utm.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ryb.jiagoushi.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynp.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sds.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://mks.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fev.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nkw.yfazqb.com

[E22] 字节长度与字符长度
来源：http://twb.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://woo.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xzj.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uwf.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hyp.aizwys.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ihy.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dwy.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://thc.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pts.tianlin.xyz

================================================================================
来源：http://jew.redwolf501.top

F. 文件与目录
来源：http://omg.wangdashe.top

================================================================================
来源：http://vgc.zhongyouzk.top

[F01] 读取整个文件
来源：http://mci.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tro.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://ith.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://luz.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uqy.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ydt.fktsv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xey.bbcook.cn

Ruby: File.read("a.txt")
来源：http://skc.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://bbw.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://dcx.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xqp.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kfx.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kbz.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ybh.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kon.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oqt.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uib.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://reb.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://nll.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fph.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gcn.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mim.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fvb.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lhc.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hxp.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://mqt.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nvr.yuanzhike.top

[F04] 追加写入文件
来源：http://jik.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://anb.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mss.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://txh.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vly.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sci.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xvl.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ktf.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gjj.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://uqw.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://irc.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://yfw.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://wum.hesvh.cn


<!-- 参考信息 -->