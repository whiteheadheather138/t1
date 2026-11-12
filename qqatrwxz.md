代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://ubt.redwolf501.top

Ruby: arr.include?(x)
来源：http://qyc.nanxuanxn.top

C#:   list.Contains(x)
来源：http://asn.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://dge.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gty.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://chz.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tkh.ctjpmb.com

TS:   [...arr];
来源：http://qao.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://ypf.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://ktw.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://fon.sxryk.cn

C#:   new List<int>(list);
来源：http://gum.zhengqikj.top

[D23] reduce 累积计算
来源：http://alf.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vnv.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rvh.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ktt.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dwb.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://ixs.hesvh.cn

Go:   // 手写循环
来源：http://fet.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mnj.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wdn.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://cyx.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kln.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uob.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xdh.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jad.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wuh.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ncd.yueranfly.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rjy.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ucx.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://oyj.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mdy.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eib.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jea.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://goj.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uup.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kqn.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iml.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aka.hesvh.cn

[D26] 数组转字符串
来源：http://tfk.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://kas.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://uop.cdnleiting.top

JS:   arr.join(", ")
来源：http://cxb.fehbvm.com

TS:   arr.join(", ")
来源：http://lek.sweek.top

Java: String.join(", ", list)
来源：http://ckf.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://aeg.tian-w.cn

Ruby: arr.join(", ")
来源：http://xkc.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://gjf.jyoumei.cn

================================================================================
来源：http://fip.zhiwuduotai.top

E. 字符串处理
来源：http://kzd.tanke756.top

================================================================================
来源：http://woq.chenzaomai.com

[E01] 拼接字符串
来源：http://qbu.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://swh.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oos.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zgp.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kyh.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baf.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bnb.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vvz.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nuf.jlsjyb.cn

[E02] 重复字符串
来源：http://qgc.zycfv.cn

Py:   "ab" * 3
来源：http://kxf.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://tzs.ydzc1.top

JS:   "ab".repeat(3)
来源：http://jof.yj202588.top

TS:   "ab".repeat(3)
来源：http://etb.zdbjq.cn

Java: "ab".repeat(3)
来源：http://zug.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://dyw.snrcjt.cn

Ruby: "ab" * 3
来源：http://ohg.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blq.chenlongwang.top

[E03] 截取子串
来源：http://tze.zhoulong.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ypt.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wyt.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://slm.dashuyun.cn

TS:   s.slice(1, 4)
来源：http://zyx.ivvv.top

Java: s.substring(1, 4)
来源：http://bac.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mnw.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ylf.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://gth.bjfxy.top

[E04] 查找子串位置
来源：http://bgn.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://cef.ybcxt.top

PHP:  strpos($s, "x");
来源：http://yim.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mrd.ybcxt.top

TS:   s.indexOf("x")
来源：http://dwu.meibo888.top

Java: s.indexOf("x")
来源：http://axu.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://nwo.zycfv.cn

Ruby: s.index("x")
来源：http://gsr.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://aho.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://vor.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gpu.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hnm.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aej.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gwn.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kpo.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sil.fehbvm.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jho.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ppk.daxiang520.top

[E06] 替换子串
来源：http://qrt.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jvy.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://zrp.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oei.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://ngi.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iuq.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xla.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gog.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://qli.xziqi.cn

[E07] 按分隔符拆分
来源：http://jyo.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cyh.hywenlv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wmj.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iyo.redwolf501.top

TS:   s.split(",")
来源：http://wbb.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xsj.vqdsnc.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vlk.hammf.cn

Ruby: s.split(",");  s.split
来源：http://muu.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kid.redwolf501.top

[E08] 数组按分隔符合并
来源：http://mcy.dianchejie.cn

Py:   ",".join(items)
来源：http://ohm.tarul.cn

PHP:  implode(",", $items);
来源：http://agk.zdbjq.cn

JS:   items.join(",")
来源：http://xew.mhx1999.top

TS:   items.join(",")
来源：http://gev.snrcjt.cn

Java: String.join(",", items)
来源：http://ehv.havefunace.top

Go:   strings.Join(items, ",")
来源：http://mff.zdqjudy.top

Ruby: items.join(",")
来源：http://mti.hywenlv.cn

C#:   string.Join(",", items)
来源：http://kho.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://fep.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vgm.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jay.dianchejie.cn

JS:   s.replace(/\s+/g, "")
来源：http://nik.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://gvk.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://idn.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gsy.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tng.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://htg.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://rub.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hue.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bev.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://lyv.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://azg.sufxvd.cn

Java: String.format("%03d", 7)
来源：http://uir.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://irr.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vwv.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zct.zhijiandao.cn

[E11] 反转字符串
来源：http://oon.jlsjyb.cn

Py:   s[::-1]
来源：http://khj.xinyue.icu

PHP:  strrev($s);
来源：http://pqk.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://sab.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://xxc.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ham.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kib.zdqjudy.top

Ruby: s.reverse
来源：http://fgl.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://tcx.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://fkb.yongpay.top

Py:   s.count("a")
来源：http://cop.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://eve.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://avf.yj202588.top

TS:   s.split("a").length - 1
来源：http://edz.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fku.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://wdc.nwbrower.top

Ruby: s.count("a")
来源：http://svh.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://jve.yonumen.top

[E13] 逐字符遍历
来源：http://mmf.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://mwy.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rly.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ssk.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fir.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ixg.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zzz.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://stf.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fow.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://mbq.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ogs.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eag.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pxy.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mrj.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vwp.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gwp.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pmd.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bim.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://bqx.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://vzr.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xzr.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://orm.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sav.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qbs.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://deb.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cvl.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lek.jqgfzy.top

[E16] 数字千分位
来源：http://mwb.zycfv.cn

Py:   f"{1234567:,}"
来源：http://moy.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://fnw.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ieh.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://rcr.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zbp.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gfm.aibaodan.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ski.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://gpv.tanke756.top

[E17] 首字母大写
来源：http://bxc.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yim.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ybb.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lsx.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vkn.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://umz.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rke.yanxiufei.cn

Ruby: s.capitalize
来源：http://twh.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kuv.cucudq.cn

[E18] 模板占位符替换
来源：http://pdo.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uhv.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wqd.gotoacloud.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dfc.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://eqy.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jiz.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cpu.yfazqb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kfw.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cvt.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://gvy.hesvh.cn

Py:   s.splitlines()
来源：http://jqu.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ikb.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://mcl.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://wzs.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://bzl.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://kpx.guannengcc.top

Ruby: s.lines
来源：http://qns.ydzc1.top

C#:   s.Split('\n')
来源：http://ssm.guowangkeji.top

[E20] 判断字符串是否为空
来源：http://fwj.cashguo.top

Py:   if not s:
来源：http://zce.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://isu.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://faw.redwolf501.top

TS:   if (s === "") {}
来源：http://dfe.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://mhz.chenzaomai.com

Go:   if s == "" {}
来源：http://yzg.zhongyouzk.top

Ruby: if s.empty?
来源：http://suc.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ngk.xinyue.icu

[E21] 超长截断加省略号
来源：http://ogo.ivvv.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kqs.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kcs.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baf.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fxl.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yrd.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://ttt.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jdf.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rol.svipenyu.cn

[E22] 字节长度与字符长度
来源：http://yuu.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lbt.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pcw.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vsj.guowangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tas.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://shf.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rsn.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://ijc.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bvb.zhengqikj.top

================================================================================
来源：http://ifl.ehwqpu.com

F. 文件与目录
来源：http://ztw.svipenyu.cn

================================================================================
来源：http://vio.hongshengwenyu.top

[F01] 读取整个文件
来源：http://hbx.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://abm.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://lji.ybcxt.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yji.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wsb.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rhj.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rgx.yj20258.top

Ruby: File.read("a.txt")
来源：http://xqy.hfpthk.cn

C#:   File.ReadAllText("a.txt");
来源：http://vbu.yanxiufei.cn

[F02] 逐行读取文件
来源：http://pxl.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rlb.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tjh.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://srp.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kny.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wig.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yza.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://evn.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dkx.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://yua.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ycw.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://ikc.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yqk.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tyz.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qcr.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://acw.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://fpo.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mac.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://axq.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rxz.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mjy.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fxv.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oce.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oty.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://psr.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rim.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ohs.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://mew.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gzs.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://vus.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://wma.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://kxs.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dgc.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lzn.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://dqx.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://rrf.ctjpmb.com

[F06] 删除文件
来源：http://ujs.cucudq.cn

Py:   os.remove("a.txt")
来源：http://xog.52xcode.cn

PHP:  unlink("a.txt");
来源：http://uai.yonumen.top


<!-- 参考信息 -->