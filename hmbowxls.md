代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://oxq.hcnkem.com

Ruby: arr.include?(x)
来源：http://bbm.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://iji.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://lis.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oug.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kzj.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://myf.shanyushiyangkeji.top

TS:   [...arr];
来源：http://npt.vehdjk.com

Java: new ArrayList<>(list);
来源：http://vvl.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://klc.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://agj.sysykeji.top

C#:   new List<int>(list);
来源：http://wpk.ivvv.top

[D23] reduce 累积计算
来源：http://mrs.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rof.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ouz.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wzp.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nsm.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gsd.nwbrower.top

Go:   // 手写循环
来源：http://tiu.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zjx.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zhe.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://wey.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vai.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qdq.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kfh.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wbu.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tmg.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eaj.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://awc.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mqg.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://wjs.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pfb.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://opu.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ccz.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://erq.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iho.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zcl.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hdu.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nmk.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://bfb.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://yjz.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://rtl.sweek.top

JS:   arr.join(", ")
来源：http://lkd.cucudq.cn

TS:   arr.join(", ")
来源：http://pco.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://lsc.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://ltu.ehwqpu.com

Ruby: arr.join(", ")
来源：http://unv.tarul.cn

C#:   string.Join(", ", list)
来源：http://iyd.chenlongwang.top

================================================================================
来源：http://fau.jinqigufen.top

E. 字符串处理
来源：http://ljw.yueranfly.top

================================================================================
来源：http://zii.tarul.cn

[E01] 拼接字符串
来源：http://jnt.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sbv.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ewg.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rxp.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfv.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nmr.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://axb.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://edu.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hpk.yueranfly.top

[E02] 重复字符串
来源：http://pxl.zdqjudy.top

Py:   "ab" * 3
来源：http://gtd.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://mbo.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://buu.mhx1999.top

TS:   "ab".repeat(3)
来源：http://cvk.smart0.xyz

Java: "ab".repeat(3)
来源：http://eli.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://rmq.yj202588.top

Ruby: "ab" * 3
来源：http://xop.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rsf.hfpthk.cn

[E03] 截取子串
来源：http://ukv.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bns.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tdt.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bll.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://uor.nanxinkj.top

Java: s.substring(1, 4)
来源：http://ywn.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dyf.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://csd.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://gzh.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://gto.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://jrk.sjlbkw.cn

PHP:  strpos($s, "x");
来源：http://fka.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bwz.9152youxi.cn

TS:   s.indexOf("x")
来源：http://yhk.sweek.top

Java: s.indexOf("x")
来源：http://qxm.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://rpn.yuxming.cn

Ruby: s.index("x")
来源：http://lol.cheryme.top

C#:   s.IndexOf("x")
来源：http://emx.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gjm.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nov.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pnb.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://csf.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gvp.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kzj.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jxw.fehbvm.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cfa.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://syh.xinyue.icu

[E06] 替换子串
来源：http://ejs.zdqjudy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mkb.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://msb.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qvf.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://onr.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hzg.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rcl.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yfv.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://wzn.wangdashe.top

[E07] 按分隔符拆分
来源：http://uud.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dcc.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gph.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://aow.zhongyouzk.top

TS:   s.split(",")
来源：http://mrv.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://kjg.9152youxi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lwo.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://umg.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kch.yongpay.top

[E08] 数组按分隔符合并
来源：http://dao.chenzaomai.com

Py:   ",".join(items)
来源：http://lxq.ppjwa.cn

PHP:  implode(",", $items);
来源：http://fsu.jinghuilouyu.cn

JS:   items.join(",")
来源：http://qnl.yuxming.cn

TS:   items.join(",")
来源：http://mnh.hnqzz.top

Java: String.join(",", items)
来源：http://ewy.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://zos.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://mit.ppjwa.cn

C#:   string.Join(",", items)
来源：http://cii.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://ssb.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qzi.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xwj.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://bid.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://pki.jqgfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://lxd.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://svi.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://igz.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qke.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://sza.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vpp.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bik.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://vwb.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://fbk.bjfxy.top

Java: String.format("%03d", 7)
来源：http://stc.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://frk.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kvz.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eds.hfpthk.cn

[E11] 反转字符串
来源：http://yhi.pengpengdd.cyou

Py:   s[::-1]
来源：http://voa.uphjek.com

PHP:  strrev($s);
来源：http://qgi.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://fbq.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://kaa.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://swd.xuetiantiany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pgs.havefunace.top

Ruby: s.reverse
来源：http://dpo.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://dko.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://kih.andypj.xyz

Py:   s.count("a")
来源：http://xsi.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://zqw.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://ucq.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://muc.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qdr.cheryme.top

Go:   strings.Count(s, "a")
来源：http://zam.chenlongwang.top

Ruby: s.count("a")
来源：http://iru.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://kgl.fehbvm.com

[E13] 逐字符遍历
来源：http://ruq.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://mzw.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wyf.mhx1999.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vxs.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dhh.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uyv.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ohg.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nti.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ins.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://hhk.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ozr.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://uvp.zycfv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cqm.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://avc.chenjidiqi.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tys.andypj.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://boh.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nuj.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ltc.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://rhx.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iqg.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qhj.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fap.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vdx.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wxp.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bfh.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://exs.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ixx.gaohongyu789.top

[E16] 数字千分位
来源：http://cip.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://nwh.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://bhe.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pzy.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ppr.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lur.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ayi.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://afl.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://axs.meibo888.top

[E17] 首字母大写
来源：http://bhz.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lzx.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://msq.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vvf.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vwc.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ztq.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://egg.jinqigfzy.top

Ruby: s.capitalize
来源：http://vgu.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sna.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://onf.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mzv.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://foz.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xbl.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://uat.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fox.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://afi.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qdq.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://agh.guannengcc.top

[E19] 多行文本按行拆分
来源：http://vfs.52xcode.cn

Py:   s.splitlines()
来源：http://hci.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ncs.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://aiq.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://jpy.andypj.xyz

Java: s.lines().toList()
来源：http://mee.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://apo.shuidangran.top

Ruby: s.lines
来源：http://oot.svipenyu.cn

C#:   s.Split('\n')
来源：http://mdn.iojbl.cn

[E20] 判断字符串是否为空
来源：http://gxc.sxryk.cn

Py:   if not s:
来源：http://ppl.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hnh.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yuh.yj202588.top

TS:   if (s === "") {}
来源：http://ebj.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://xpx.9152youxi.cn

Go:   if s == "" {}
来源：http://ipb.cashguo.top

Ruby: if s.empty?
来源：http://vjr.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mlc.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://kdg.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jas.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kjn.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rbm.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fme.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qju.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://bqy.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ckg.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://igw.daxiang520.top

[E22] 字节长度与字符长度
来源：http://enp.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yxv.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://myd.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kup.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xpw.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tri.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dgg.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://tka.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hyw.9152youxi.cn

================================================================================
来源：http://ens.xuanzx.com

F. 文件与目录
来源：http://lkf.guowangkeji.top

================================================================================
来源：http://asc.zdqjudy.top

[F01] 读取整个文件
来源：http://rkw.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://smk.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://msq.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wel.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vll.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gbo.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mbw.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://ied.hfpthk.cn

C#:   File.ReadAllText("a.txt");
来源：http://hlx.gotoacloud.top

[F02] 逐行读取文件
来源：http://ktq.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pen.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://egq.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lwc.ywan-chungtsiang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uzo.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://shr.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cku.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xly.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wwr.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://lfv.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gyy.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cgy.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ysb.kuanghao11.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pus.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fgs.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ehr.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://qwi.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ted.hysaishi.cn

[F04] 追加写入文件
来源：http://nbr.cqqwz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rfj.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yuu.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zlr.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://agk.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ssv.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lxd.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ghw.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gyr.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://hnw.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zjg.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://ohi.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://xch.shzxlz.cn

TS:   fs.existsSync("a.txt")
来源：http://ylm.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sje.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qjz.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://azc.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://ict.xinyue.icu

[F06] 删除文件
来源：http://kkw.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://scq.yangfankeji.com

PHP:  unlink("a.txt");
来源：http://nol.hesvh.cn


<!-- 参考信息 -->