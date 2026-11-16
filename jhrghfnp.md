代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://wdj.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nta.zdqjudy.top

Go:   // 手写 map[string][]T
来源：http://pbq.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gzi.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lzb.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://tuo.yj202588.top

Py:   Counter(arr)
来源：http://xqt.xuanzx.com

PHP:  array_count_values($arr);
来源：http://sol.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://abl.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ein.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rmz.52xcode.cn

Go:   // 手写 map[T]int
来源：http://tky.sxryk.cn

Ruby: arr.tally
来源：http://zzi.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kjk.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://tij.aizwys.cn

Py:   x in arr
来源：http://icq.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://uok.cucudq.cn

JS:   arr.includes(x)
来源：http://dpu.dashuyun.cn

TS:   arr.includes(x)
来源：http://xwb.ctjpmb.com

Java: list.contains(x)
来源：http://mge.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://eja.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://fjs.vehdjk.com

C#:   list.Contains(x)
来源：http://udh.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://wyg.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tfn.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cha.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jbc.havefunace.top

TS:   [...arr];
来源：http://ieg.yj20258.top

Java: new ArrayList<>(list);
来源：http://kbp.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://clr.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://hki.xziqi.cn

C#:   new List<int>(list);
来源：http://uhx.zhengqikj.top

[D23] reduce 累积计算
来源：http://xaf.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yqr.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vgv.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vwj.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xjd.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rdn.bjfxy.top

Go:   // 手写循环
来源：http://kto.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ibf.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mba.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://cdk.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ejb.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://goe.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mxt.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hfw.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fao.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kiy.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://czh.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sxn.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://abp.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cto.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lvk.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lsh.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ewo.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nub.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dxq.yj202588.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kbu.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wnc.zhijiandao.cn

[D26] 数组转字符串
来源：http://onk.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://bam.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://lpu.ehwqpu.com

JS:   arr.join(", ")
来源：http://rvq.nanxinkj.top

TS:   arr.join(", ")
来源：http://grq.sjlbkw.cn

Java: String.join(", ", list)
来源：http://gcz.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://ieu.52xcode.cn

Ruby: arr.join(", ")
来源：http://ezp.uphjek.com

C#:   string.Join(", ", list)
来源：http://onu.jianghu66.top

================================================================================
来源：http://ahw.snrcjt.cn

E. 字符串处理
来源：http://rvi.guannengcc.top

================================================================================
来源：http://kjx.zdqjudy.top

[E01] 拼接字符串
来源：http://hae.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wpq.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mez.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oqs.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lqr.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cng.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xao.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ijl.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mop.zhijiandao.cn

[E02] 重复字符串
来源：http://obz.zdqjudy.top

Py:   "ab" * 3
来源：http://gvd.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://nzd.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://jls.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://pnl.fzhhl.top

Java: "ab".repeat(3)
来源：http://qnu.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://muh.hfpthk.cn

Ruby: "ab" * 3
来源：http://lud.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ubn.cqqwz.cn

[E03] 截取子串
来源：http://cvg.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://spa.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oum.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lkz.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://wxu.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://erf.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xbz.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hwd.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://ddo.zhijiandao.cn

[E04] 查找子串位置
来源：http://qan.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://ktf.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://lgz.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pog.cheryme.top

TS:   s.indexOf("x")
来源：http://oor.wangdashe.top

Java: s.indexOf("x")
来源：http://wgs.yvedp.cn

Go:   strings.Index(s, "x")
来源：http://tdl.zycfv.cn

Ruby: s.index("x")
来源：http://cgt.hcnkem.com

C#:   s.IndexOf("x")
来源：http://ibk.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://trz.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gjs.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mxe.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyc.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nfi.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wlo.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yok.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qjl.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gzu.sweek.top

[E06] 替换子串
来源：http://npf.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jba.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://ysz.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ygt.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://fnl.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ogl.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bmc.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://avf.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://euw.mhx1999.top

[E07] 按分隔符拆分
来源：http://bae.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jad.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rcq.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xzq.fktsv.cn

TS:   s.split(",")
来源：http://wlv.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://ctj.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ykv.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://adb.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gwr.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://rbg.fktsv.cn

Py:   ",".join(items)
来源：http://irx.birdmap.top

PHP:  implode(",", $items);
来源：http://onq.xuetiantiany.cn

JS:   items.join(",")
来源：http://kfs.hcnkem.com

TS:   items.join(",")
来源：http://qgj.0kj1m.cn

Java: String.join(",", items)
来源：http://iuh.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://tju.bbcook.cn

Ruby: items.join(",")
来源：http://pfr.epnwcf.com

C#:   string.Join(",", items)
来源：http://fnn.birdmap.top

[E09] 去除所有空白字符
来源：http://hzj.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ynh.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iyf.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://gjk.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://lxu.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://mfc.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mgt.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://kzb.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vhp.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://mzo.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ncf.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ieq.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://qip.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://asg.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://rwg.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zbm.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rsb.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nxc.c1oappe.top

[E11] 反转字符串
来源：http://spa.jinqigufen.top

Py:   s[::-1]
来源：http://xwj.fanxiaobao.xyz

PHP:  strrev($s);
来源：http://ire.pycfn.com

JS:   [...s].reverse().join("")
来源：http://dds.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://iof.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mwi.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rlu.316326.xyz

Ruby: s.reverse
来源：http://jps.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://ork.tarul.cn

[E12] 统计某字符出现次数
来源：http://xse.andypj.xyz

Py:   s.count("a")
来源：http://xes.316326.xyz

PHP:  substr_count($s, "a");
来源：http://kkk.redwolf501.top

JS:   s.split("a").length - 1
来源：http://mif.meibo888.top

TS:   s.split("a").length - 1
来源：http://oih.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vue.hammf.cn

Go:   strings.Count(s, "a")
来源：http://nma.hnxiangtu.top

Ruby: s.count("a")
来源：http://bsr.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://miu.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://ics.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://heg.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sep.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hig.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lej.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hjt.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wjk.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://enf.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ylv.zdqjudy.top

[E14] URL 编码与 Base64
来源：http://zin.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fms.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fcj.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yda.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rwh.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vkn.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://veq.yonumen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dvx.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fsk.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://pye.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pma.daria6918.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hec.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fuq.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rhy.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vkw.meibo888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dyp.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zud.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wdq.0kj1m.cn

[E16] 数字千分位
来源：http://nbb.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://bpo.xinyue.icu

PHP:  number_format(1234567);
来源：http://bbz.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nkz.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://phs.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://atw.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ayi.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://thu.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://eht.dianchejie.cn

[E17] 首字母大写
来源：http://fzm.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kyv.zhengqikj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jum.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iwv.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://moz.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xhv.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xkf.cucudq.cn

Ruby: s.capitalize
来源：http://arz.jiagoushi.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dwc.yj20258888.top

[E18] 模板占位符替换
来源：http://wxb.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jrg.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://roc.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pfa.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bgv.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xoz.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tmb.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lls.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hsu.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://ill.zycfv.cn

Py:   s.splitlines()
来源：http://gab.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sag.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://kak.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://isr.316326.xyz

Java: s.lines().toList()
来源：http://wtg.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://hkc.iojbl.cn

Ruby: s.lines
来源：http://lgy.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://mmf.aizwys.cn

[E20] 判断字符串是否为空
来源：http://onb.yanxiufei.cn

Py:   if not s:
来源：http://mwk.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wkp.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sno.9152youxi.cn

TS:   if (s === "") {}
来源：http://pfb.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://ufb.pengpengdd.cyou

Go:   if s == "" {}
来源：http://rlo.chenjidiqi.icu

Ruby: if s.empty?
来源：http://lll.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zjl.52xcode.cn

[E21] 超长截断加省略号
来源：http://vbk.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lcc.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hfp.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mlf.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dvv.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pnv.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://aks.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rgl.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ddd.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://aee.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lyj.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dfs.epnwcf.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oma.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xho.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gct.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hsw.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://qvo.sysykeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://viu.shzxlz.cn

================================================================================
来源：http://xpx.mhx1999.top

F. 文件与目录
来源：http://bou.tianlin.xyz

================================================================================
来源：http://gar.yj20258888.top

[F01] 读取整个文件
来源：http://dqt.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jtw.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://jfn.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rdv.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ses.jqgufenzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://giz.hcnkem.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fll.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://gut.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://yzl.zdbjq.cn

[F02] 逐行读取文件
来源：http://khk.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dbl.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qju.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xsk.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xvx.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pmn.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dds.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zbl.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sdc.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://dhj.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://trm.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://fpc.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tta.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rjb.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://klf.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nlq.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://toy.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qjx.gzhubu.top

[F04] 追加写入文件
来源：http://les.sysykeji.top


<!-- 参考信息 -->