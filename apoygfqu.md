代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://uis.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://iao.tarul.cn

C#:   list.Contains(x)
来源：http://aju.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://trw.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xxi.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://huc.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ami.hywenlv.cn

TS:   [...arr];
来源：http://mcj.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://abr.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://szh.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://suz.c1oappe.top

C#:   new List<int>(list);
来源：http://fta.sxryk.cn

[D23] reduce 累积计算
来源：http://puz.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pnq.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jht.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mec.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rhz.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://feq.sxryk.cn

Go:   // 手写循环
来源：http://qli.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://guj.ctjpmb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uuw.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://foi.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://axv.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://doz.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jtq.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rxm.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mbc.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ivz.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vsq.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hot.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://hdl.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kmo.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ilr.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://krq.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mmc.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uia.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sxi.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mzk.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jiu.jinqigfzy.top

[D26] 数组转字符串
来源：http://pea.jinqigfzy.top

Py:   ", ".join(map(str, arr))
来源：http://rpc.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://fvw.yj20258.top

JS:   arr.join(", ")
来源：http://hor.ehwqpu.com

TS:   arr.join(", ")
来源：http://fan.gaohongyu789.top

Java: String.join(", ", list)
来源：http://izl.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://rzi.meibo888.top

Ruby: arr.join(", ")
来源：http://wml.cucudq.cn

C#:   string.Join(", ", list)
来源：http://ejp.vehdjk.com

================================================================================
来源：http://ltd.daxiang520.top

E. 字符串处理
来源：http://aeb.zhijiandao.cn

================================================================================
来源：http://oum.zhongyouzk.top

[E01] 拼接字符串
来源：http://tck.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jqg.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qkw.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mie.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nqn.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yab.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sck.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dgk.quarkkingdee.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jkf.meibo888.top

[E02] 重复字符串
来源：http://avx.tianlin.xyz

Py:   "ab" * 3
来源：http://hok.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://fuc.sysykeji.top

JS:   "ab".repeat(3)
来源：http://bbh.zhengqikj.top

TS:   "ab".repeat(3)
来源：http://yxi.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://ydf.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://izf.hesvh.cn

Ruby: "ab" * 3
来源：http://lnz.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cip.hnqzz.top

[E03] 截取子串
来源：http://arc.hnqzz.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tdc.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wgu.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://poi.hnqzz.top

TS:   s.slice(1, 4)
来源：http://kwh.zdqjudy.top

Java: s.substring(1, 4)
来源：http://zpw.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yxl.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ewx.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://ewc.sysykeji.top

[E04] 查找子串位置
来源：http://oyx.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://cre.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://mgz.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hzl.zdqjudy.top

TS:   s.indexOf("x")
来源：http://wxg.c1oappe.top

Java: s.indexOf("x")
来源：http://jnd.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://qcq.birdmap.top

Ruby: s.index("x")
来源：http://ymp.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://knl.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zbt.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wug.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xmj.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxe.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://svc.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kyk.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://drv.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sct.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dly.wangdashe.top

[E06] 替换子串
来源：http://ier.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yyh.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://nxg.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mpm.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://ovm.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sou.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wdt.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mgs.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://vjh.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://hhm.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jnj.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sgu.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://occ.hesvh.cn

TS:   s.split(",")
来源：http://upt.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://cdb.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dce.hongshengwenyu.top

Ruby: s.split(",");  s.split
来源：http://rfp.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vhf.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://pft.iojbl.cn

Py:   ",".join(items)
来源：http://mua.yj202588.top

PHP:  implode(",", $items);
来源：http://nbh.sxryk.cn

JS:   items.join(",")
来源：http://xto.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://cai.hnqzz.top

Java: String.join(",", items)
来源：http://dhf.sweek.top

Go:   strings.Join(items, ",")
来源：http://uyo.daria6918.cn

Ruby: items.join(",")
来源：http://iju.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://mcb.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://bht.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fra.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://stp.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://stq.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://kwq.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://njm.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tyj.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://dlu.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vce.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://cvi.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zuv.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jbu.dianchejie.cn

JS:   "7".padStart(3, "0")
来源：http://sci.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://czn.aizwys.cn

Java: String.format("%03d", 7)
来源：http://per.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://adq.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yql.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jlt.cashguo.top

[E11] 反转字符串
来源：http://wke.fengsongda.top

Py:   s[::-1]
来源：http://yax.yongpay.top

PHP:  strrev($s);
来源：http://jfl.yongpay.top

JS:   [...s].reverse().join("")
来源：http://xvz.pycfn.com

TS:   [...s].reverse().join("")
来源：http://enj.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aia.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tkj.sysykeji.top

Ruby: s.reverse
来源：http://cxe.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ksu.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://rlm.hnxiangtu.top

Py:   s.count("a")
来源：http://ble.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://sqv.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://iqn.smart0.xyz

TS:   s.split("a").length - 1
来源：http://kdj.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wxj.cheryme.top

Go:   strings.Count(s, "a")
来源：http://htx.daria6918.cn

Ruby: s.count("a")
来源：http://zir.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://bdh.hnxiangtu.top

[E13] 逐字符遍历
来源：http://cxm.yonumen.top

Py:   for ch in s: print(ch)
来源：http://nmh.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://osa.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kmv.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ogh.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wtf.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ddl.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kyq.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kcg.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://puy.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zuj.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://buz.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ooy.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://clt.ydjk.org.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rwk.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rme.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sgw.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tko.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://nup.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nrz.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ucd.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nxv.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fdl.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ioi.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sip.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ewo.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lyo.vehdjk.com

[E16] 数字千分位
来源：http://ful.hcnkem.com

Py:   f"{1234567:,}"
来源：http://ohd.aizwys.cn

PHP:  number_format(1234567);
来源：http://txx.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kka.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://sjh.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wci.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lmh.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dbh.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://hoe.cqqwz.cn

[E17] 首字母大写
来源：http://ato.zycfv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fvt.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://zjm.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vys.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yeo.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gpo.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://djj.tanke756.top

Ruby: s.capitalize
来源：http://ysx.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hht.ybcxt.top

[E18] 模板占位符替换
来源：http://ecn.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ixr.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gst.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://elv.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jwp.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kat.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://orn.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uft.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mjr.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://bse.guowangkeji.top

Py:   s.splitlines()
来源：http://lcy.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bqg.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://djq.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://qnk.yangfankeji.com

Java: s.lines().toList()
来源：http://psn.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://hsu.gzhubu.top

Ruby: s.lines
来源：http://ebz.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://ymc.ivvv.top

[E20] 判断字符串是否为空
来源：http://mdd.dianchejie.cn

Py:   if not s:
来源：http://qrd.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wpv.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://syl.cdnleiting.top

TS:   if (s === "") {}
来源：http://qnl.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://dep.jqgufenzy.top

Go:   if s == "" {}
来源：http://icf.xinyue.icu

Ruby: if s.empty?
来源：http://xab.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hqq.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://lrg.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hyo.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fqg.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uhm.aizwys.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dpo.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://imr.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://yeh.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pmb.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zzk.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://xzy.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rcx.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ztg.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fsl.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wgl.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rqc.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qhc.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://sdi.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gzu.shanyushiyangkeji.top

================================================================================
来源：http://cte.cheryme.top

F. 文件与目录
来源：http://ndu.shzxlz.cn

================================================================================
来源：http://qkx.ydjk.org.cn

[F01] 读取整个文件
来源：http://fym.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://say.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://rjj.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hxn.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rvv.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cgd.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pfb.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://zid.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://ffv.vehdjk.com

[F02] 逐行读取文件
来源：http://bhn.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bzv.jqgfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kpf.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dct.sysykeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rfv.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zfi.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dip.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bro.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tbl.ivvv.top

[F03] 写入文件（覆盖）
来源：http://ftk.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kas.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://clf.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uvp.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ukg.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dfc.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uza.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://dyu.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ssh.yueranfly.top

[F04] 追加写入文件
来源：http://kci.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://knu.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fzw.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://thh.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zjp.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zha.zycfv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://izw.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://phk.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hxp.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://lbi.yueranfly.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gnz.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://ogo.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://thn.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://qog.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://uik.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dmd.sweek.top

Ruby: File.exist?("a.txt")
来源：http://hcj.yonumen.top

C#:   File.Exists("a.txt")
来源：http://tla.yuanzhike.top

[F06] 删除文件
来源：http://nrn.cheryme.top

Py:   os.remove("a.txt")
来源：http://ujs.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://bat.sufxvd.cn


<!-- 参考信息 -->