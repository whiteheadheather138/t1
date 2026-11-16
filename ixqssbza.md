代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nhm.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://env.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ves.iojbl.cn

Go:   // 手写 map[T]int
来源：http://ikq.nanxinkj.top

Ruby: arr.tally
来源：http://zdi.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uxz.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://whi.tianlin.xyz

Py:   x in arr
来源：http://oct.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://iae.xuanzx.com

JS:   arr.includes(x)
来源：http://bgu.zhoulong.xyz

TS:   arr.includes(x)
来源：http://shi.fktsv.cn

Java: list.contains(x)
来源：http://jef.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://rww.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://fop.c1oappe.top

C#:   list.Contains(x)
来源：http://qhg.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://jmk.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zgv.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nlu.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lxa.cdnleiting.top

TS:   [...arr];
来源：http://xkd.havefunace.top

Java: new ArrayList<>(list);
来源：http://oog.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bso.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://psm.daria6918.cn

C#:   new List<int>(list);
来源：http://jvo.zdqjudy.top

[D23] reduce 累积计算
来源：http://dlj.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qrw.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dda.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iyx.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tyd.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pog.snrcjt.cn

Go:   // 手写循环
来源：http://ogm.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lpl.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mdj.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://jcz.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rgw.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kep.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rmy.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kpj.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ive.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cfw.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yvr.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dfj.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://grq.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rtc.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yla.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://krp.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://abs.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cut.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://etf.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tno.chenlongwang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rak.svipenyu.cn

[D26] 数组转字符串
来源：http://prt.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://zzy.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://moc.gaohongyu789.top

JS:   arr.join(", ")
来源：http://upv.zdbjq.cn

TS:   arr.join(", ")
来源：http://okv.ybcxt.top

Java: String.join(", ", list)
来源：http://ecs.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://onc.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://xry.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://hoo.daria6918.cn

================================================================================
来源：http://adw.jiagoushi.top

E. 字符串处理
来源：http://uzk.epnwcf.com

================================================================================
来源：http://omh.zhijiandao.cn

[E01] 拼接字符串
来源：http://bvq.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ujx.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bqh.jyoumei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://znv.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pvw.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pig.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://prh.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://onv.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hcm.yonumen.top

[E02] 重复字符串
来源：http://rca.kuanghao11.cn

Py:   "ab" * 3
来源：http://mrm.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://ybh.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://idp.redwolf501.top

TS:   "ab".repeat(3)
来源：http://exb.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://yjx.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://pyz.daria6918.cn

Ruby: "ab" * 3
来源：http://sdl.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rce.hywenlv.cn

[E03] 截取子串
来源：http://dyi.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mma.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xeh.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ujv.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://crn.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://dfq.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mal.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yfv.yonumen.top

C#:   s.Substring(1, 3)
来源：http://yea.dianchejie.cn

[E04] 查找子串位置
来源：http://ojs.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://kaf.hesvh.cn

PHP:  strpos($s, "x");
来源：http://xqg.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cvb.sysykeji.top

TS:   s.indexOf("x")
来源：http://dhz.zycfv.cn

Java: s.indexOf("x")
来源：http://cyj.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://wqg.yangfankeji.com

Ruby: s.index("x")
来源：http://fwn.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://ebl.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://eyt.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lbp.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kim.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vsy.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jvs.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akv.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gyl.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lbe.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gaq.sjlbkw.cn

[E06] 替换子串
来源：http://epc.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vsj.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://wvq.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gru.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://btu.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uou.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ahz.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zxv.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://ocs.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://qqf.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ldr.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lcj.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ulo.vehdjk.com

TS:   s.split(",")
来源：http://cjc.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xtq.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ttf.xuetiantiany.cn

Ruby: s.split(",");  s.split
来源：http://plo.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lho.epnwcf.com

[E08] 数组按分隔符合并
来源：http://fzu.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://ogs.daxiang520.top

PHP:  implode(",", $items);
来源：http://zhn.sjlbkw.cn

JS:   items.join(",")
来源：http://vkb.yuanzhike.top

TS:   items.join(",")
来源：http://xzk.nanxinkj.top

Java: String.join(",", items)
来源：http://oxa.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://bdg.fengsongda.top

Ruby: items.join(",")
来源：http://yyf.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://jvg.yj20258.top

[E09] 去除所有空白字符
来源：http://qcq.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sng.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rig.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://vzj.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://nyf.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://wus.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vfq.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://knc.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sht.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://siy.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ttz.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rvf.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://ips.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://ila.yvedp.cn

Java: String.format("%03d", 7)
来源：http://che.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://otm.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bmx.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rzf.dashuyun.cn

[E11] 反转字符串
来源：http://unj.0kj1m.cn

Py:   s[::-1]
来源：http://zas.zhongyouzk.top

PHP:  strrev($s);
来源：http://fdv.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://rtp.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://tff.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gic.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qez.zhoulong.xyz

Ruby: s.reverse
来源：http://nad.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://upe.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://lez.zhijiandao.cn

Py:   s.count("a")
来源：http://nrd.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://pmb.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://sqz.smart0.xyz

TS:   s.split("a").length - 1
来源：http://atf.sysykeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nnr.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://fxe.cheryme.top

Ruby: s.count("a")
来源：http://nju.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://jcy.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://eji.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://shi.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yxz.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bez.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://byl.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fmv.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uxr.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://utg.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jha.fzhhl.top

[E14] URL 编码与 Base64
来源：http://aqw.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dlu.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sux.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hlo.cucudq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bju.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://txa.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tll.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lor.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wgj.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://dmv.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ncm.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dwd.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xhc.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://qpd.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kjb.xylfe.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ohn.jinqigfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ukr.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qvx.zhiwuduotai.top

[E16] 数字千分位
来源：http://dot.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://qdu.xinyue.icu

PHP:  number_format(1234567);
来源：http://opk.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kim.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lud.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eie.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vwm.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zuf.tanke756.top

C#:   1234567.ToString("N0")
来源：http://qzi.redwolf501.top

[E17] 首字母大写
来源：http://nhb.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mzs.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lkx.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzu.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://stt.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hjz.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rpm.bbcook.cn

Ruby: s.capitalize
来源：http://zfg.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://epg.bbcook.cn

[E18] 模板占位符替换
来源：http://sru.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wmr.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uun.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://tvl.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ulw.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vxp.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://thm.yfazqb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lwv.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://adu.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://aub.hongshengwenyu.top

Py:   s.splitlines()
来源：http://pwr.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rfs.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://hbz.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://hub.yangfankeji.com

Java: s.lines().toList()
来源：http://nrx.yongpay.top

Go:   strings.Split(s, "\n")
来源：http://xla.jqgfzy.top

Ruby: s.lines
来源：http://dzn.fzhhl.top

C#:   s.Split('\n')
来源：http://tdf.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://jmq.yj20258888.top

Py:   if not s:
来源：http://dqx.epnwcf.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ixg.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pmr.kuanghao11.cn

TS:   if (s === "") {}
来源：http://ujb.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://exn.guowangkeji.top

Go:   if s == "" {}
来源：http://nvq.vqdsnc.cn

Ruby: if s.empty?
来源：http://rfr.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://svq.chenzaomai.com

[E21] 超长截断加省略号
来源：http://lov.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pdi.tianlin.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ofr.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sxt.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gbo.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://etf.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://xlz.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bup.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jfo.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://abt.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dgg.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bkh.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lxg.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://asl.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ura.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cah.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://olj.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cfx.zdqjudy.top

================================================================================
来源：http://efx.316326.xyz

F. 文件与目录
来源：http://rma.meibo888.top

================================================================================
来源：http://vei.cucudq.cn

[F01] 读取整个文件
来源：http://yyo.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fvk.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://bdx.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cru.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zdw.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xwd.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://god.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://mhl.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://mtq.xziqi.cn

[F02] 逐行读取文件
来源：http://xpk.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hht.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xfo.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bqq.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zlu.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ygm.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mqb.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mav.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rby.yj20258.top

[F03] 写入文件（覆盖）
来源：http://ewf.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pqh.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://evl.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ibq.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vek.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uyc.ydzc1.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mzn.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://jfw.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nqb.gaohongyu789.top

[F04] 追加写入文件
来源：http://oyh.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ppo.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dqc.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xvm.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ric.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fhv.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://abd.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zer.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zac.meibo888.top


<!-- 参考信息 -->