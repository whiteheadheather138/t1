代发 wailian999

Ruby: arr.tally
来源：http://muo.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ndl.ybcxt.top

[D21] 判断是否包含某元素
来源：http://pkq.chenjidiqi.icu

Py:   x in arr
来源：http://imy.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://kwm.fktsv.cn

JS:   arr.includes(x)
来源：http://unt.sysykeji.top

TS:   arr.includes(x)
来源：http://adk.jinghuilouyu.cn

Java: list.contains(x)
来源：http://yev.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://xvb.bjfxy.top

Ruby: arr.include?(x)
来源：http://ohn.gaohongyu789.top

C#:   list.Contains(x)
来源：http://zyv.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://qup.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://llw.birdmap.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hwb.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tle.hywenlv.cn

TS:   [...arr];
来源：http://klv.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://cca.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hhv.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://pbv.fengsongda.top

C#:   new List<int>(list);
来源：http://ptg.bjfxy.top

[D23] reduce 累积计算
来源：http://fdn.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pln.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jia.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sfy.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jxm.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://tuj.guannengcc.top

Go:   // 手写循环
来源：http://msr.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xdn.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qdn.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://oic.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://waj.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wzt.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ijn.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uda.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cjl.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cqp.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://klk.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fsu.havefunace.top

[D25] Set 集合去重与交并差
来源：http://hor.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ywj.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://psh.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dno.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://arj.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ncg.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ydl.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xrp.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tjc.sxryk.cn

[D26] 数组转字符串
来源：http://bxu.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://ovz.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://mky.dashuyun.cn

JS:   arr.join(", ")
来源：http://ygb.fktsv.cn

TS:   arr.join(", ")
来源：http://azc.yueranfly.top

Java: String.join(", ", list)
来源：http://mll.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://mkn.dianchejie.cn

Ruby: arr.join(", ")
来源：http://tkq.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://imy.snrcjt.cn

================================================================================
来源：http://pyy.yangfankeji.com

E. 字符串处理
来源：http://jds.cashguo.top

================================================================================
来源：http://oag.birdmap.top

[E01] 拼接字符串
来源：http://uql.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ufs.shuidangran.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lya.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fec.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xfk.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uav.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rce.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qxq.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cxd.zdbjq.cn

[E02] 重复字符串
来源：http://jsi.fehbvm.com

Py:   "ab" * 3
来源：http://yty.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://hjy.c1oappe.top

JS:   "ab".repeat(3)
来源：http://xoa.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://nfp.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://ulq.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://twi.ppjwa.cn

Ruby: "ab" * 3
来源：http://cod.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tpl.jianghu66.top

[E03] 截取子串
来源：http://xkw.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://szb.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pnz.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jbw.hesvh.cn

TS:   s.slice(1, 4)
来源：http://hqc.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://kzt.chenlongwang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vpv.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://spd.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://xzn.daxiang520.top

[E04] 查找子串位置
来源：http://mfp.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://sps.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://yov.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oun.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://mod.pengpengdd.cyou

Java: s.indexOf("x")
来源：http://coa.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://jll.gzhubu.top

Ruby: s.index("x")
来源：http://rte.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://fui.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qsh.jinqigufen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rpf.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xzm.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mdd.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vuj.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bgo.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hkr.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://arg.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zzj.cashguo.top

[E06] 替换子串
来源：http://wdq.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ltw.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://apc.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tey.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://rxi.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ztq.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://psj.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nmm.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://gwx.shzxlz.cn

[E07] 按分隔符拆分
来源：http://kdy.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xzn.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oqc.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bsh.mhx1999.top

TS:   s.split(",")
来源：http://rkf.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cru.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://esk.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://eio.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://njb.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://yvj.mhx1999.top

Py:   ",".join(items)
来源：http://phj.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://xtp.gotoacloud.top

JS:   items.join(",")
来源：http://afr.sysykeji.top

TS:   items.join(",")
来源：http://wzh.tanke756.top

Java: String.join(",", items)
来源：http://moj.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://kjq.ppjwa.cn

Ruby: items.join(",")
来源：http://rss.ydzc1.top

C#:   string.Join(",", items)
来源：http://dfo.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://xlp.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pwh.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rms.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://niv.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://jpc.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://jgy.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://hkl.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hdr.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rgq.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://las.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nil.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zqm.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://ixh.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://gpf.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://wwu.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fsk.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vkb.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://saj.yonumen.top

[E11] 反转字符串
来源：http://ulj.cdnleiting.top

Py:   s[::-1]
来源：http://nfk.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://rpj.yj20258.top

JS:   [...s].reverse().join("")
来源：http://tpk.sysykeji.top

TS:   [...s].reverse().join("")
来源：http://rhu.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://jnl.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rsh.hywenlv.cn

Ruby: s.reverse
来源：http://ela.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://goy.hammf.cn

[E12] 统计某字符出现次数
来源：http://tdw.kuanghao11.cn

Py:   s.count("a")
来源：http://ppl.hammf.cn

PHP:  substr_count($s, "a");
来源：http://elv.hesvh.cn

JS:   s.split("a").length - 1
来源：http://hdf.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://bvz.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dot.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://myn.xuanzx.com

Ruby: s.count("a")
来源：http://cuj.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://edd.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://qbz.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://vfi.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bam.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://noi.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zgb.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wfu.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aqg.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ytk.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pxz.havefunace.top

[E14] URL 编码与 Base64
来源：http://fiu.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tlw.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kbq.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ksz.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yxg.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uha.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yti.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jzy.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wlt.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://yyb.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gci.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tyu.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vcm.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://haf.ydjk.org.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nft.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eos.hammf.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gmg.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zwr.xuanzx.com

[E16] 数字千分位
来源：http://iuy.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://phq.hnqzz.top

PHP:  number_format(1234567);
来源：http://bri.haohaochexian.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bzw.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ybk.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gyb.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ixz.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tyk.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://xhx.jianghu66.top

[E17] 首字母大写
来源：http://zrt.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cmq.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bsz.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pty.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jlf.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wjp.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://olt.ydjk.org.cn

Ruby: s.capitalize
来源：http://ccb.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://duu.daria6918.cn

[E18] 模板占位符替换
来源：http://sbv.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vxb.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ajt.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vdu.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qyn.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zvb.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jss.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jzj.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nxn.yonumen.top

[E19] 多行文本按行拆分
来源：http://pmn.yvedp.cn

Py:   s.splitlines()
来源：http://fua.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://viv.sweek.top

JS:   s.split(/\r?\n/)
来源：http://tca.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://qgz.tanke756.top

Java: s.lines().toList()
来源：http://guf.hongshengwenyu.top

Go:   strings.Split(s, "\n")
来源：http://zpp.zhaomingkeji.xyz

Ruby: s.lines
来源：http://byt.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://sxp.snrcjt.cn

[E20] 判断字符串是否为空
来源：http://qfh.gogol.net.cn

Py:   if not s:
来源：http://eme.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ijb.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tcw.hcnkem.com

TS:   if (s === "") {}
来源：http://ayh.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://yck.vqdsnc.cn

Go:   if s == "" {}
来源：http://zhv.chenlongwang.top

Ruby: if s.empty?
来源：http://sqg.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kjo.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://iod.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hwu.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wlt.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pgv.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wum.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tqb.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://prn.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nnh.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kxn.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://uas.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vqs.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ues.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uvb.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xpq.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://shs.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bvm.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://bgf.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://soh.nwbrower.top

================================================================================
来源：http://ewo.shanyushiyangkeji.top

F. 文件与目录
来源：http://jzb.xinyue.icu

================================================================================
来源：http://dgg.jianghu66.top

[F01] 读取整个文件
来源：http://tzj.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oov.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://xtx.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xrl.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nix.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rbn.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wbi.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://yzd.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://mzn.hammf.cn

[F02] 逐行读取文件
来源：http://zkk.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mzc.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ytb.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqv.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cov.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kfm.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hpf.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nxf.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vrv.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://xox.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pza.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fvl.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qgk.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hbw.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://twd.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gtg.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://glz.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yue.cheryme.top

[F04] 追加写入文件
来源：http://sps.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wsc.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mni.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dfy.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wqs.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rud.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rzs.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://huh.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://epi.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://rna.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xnu.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://nif.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://hhu.kuanghao11.cn


<!-- 参考信息 -->