代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uru.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://apm.chenlongwang.top

Py:   Counter(arr)
来源：http://oxo.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://qwk.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wri.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qgz.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mpk.uphjek.com

Go:   // 手写 map[T]int
来源：http://xhh.zhiwuduotai.top

Ruby: arr.tally
来源：http://qxs.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tmp.tarul.cn

[D21] 判断是否包含某元素
来源：http://pjz.9152youxi.cn

Py:   x in arr
来源：http://fzb.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://ruh.0kj1m.cn

JS:   arr.includes(x)
来源：http://byh.yj20258.top

TS:   arr.includes(x)
来源：http://aln.ivvv.top

Java: list.contains(x)
来源：http://tni.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://eka.haohaochexian.top

Ruby: arr.include?(x)
来源：http://xco.chenzaomai.com

C#:   list.Contains(x)
来源：http://mgx.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://hoq.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sfq.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qxk.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jqn.shuidangran.top

TS:   [...arr];
来源：http://ala.sweek.top

Java: new ArrayList<>(list);
来源：http://ypf.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pul.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://faz.ivvv.top

C#:   new List<int>(list);
来源：http://tci.tanke756.top

[D23] reduce 累积计算
来源：http://okd.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dwq.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hic.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bft.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://abw.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rfg.yfazqb.com

Go:   // 手写循环
来源：http://qdc.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://amj.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qqj.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://rgo.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ibv.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://owq.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://toa.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qmb.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wtf.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eta.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://shu.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gfo.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://fmx.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://olh.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://swj.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fav.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://plj.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zpb.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jmd.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kya.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bgh.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://gpv.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://nvk.ivvv.top

PHP:  implode(", ", $arr);
来源：http://wfa.haohaochexian.top

JS:   arr.join(", ")
来源：http://tqm.xuanzx.com

TS:   arr.join(", ")
来源：http://wvn.yj20258888.top

Java: String.join(", ", list)
来源：http://rlr.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://jwm.tian-w.cn

Ruby: arr.join(", ")
来源：http://ikr.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://hvf.xziqi.cn

================================================================================
来源：http://hwt.jlsjyb.cn

E. 字符串处理
来源：http://xrv.zhengqikj.top

================================================================================
来源：http://qma.zhiwuduotai.top

[E01] 拼接字符串
来源：http://thh.gaohongyu789.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://viv.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jwx.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qhq.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnk.aibaodan.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aqq.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oug.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ihi.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zsz.tarul.cn

[E02] 重复字符串
来源：http://tlq.tanke756.top

Py:   "ab" * 3
来源：http://fpi.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://tjd.yongpay.top

JS:   "ab".repeat(3)
来源：http://rol.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://dzn.fktsv.cn

Java: "ab".repeat(3)
来源：http://fgb.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://jyh.zhongyouzk.top

Ruby: "ab" * 3
来源：http://cay.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iif.sjlbkw.cn

[E03] 截取子串
来源：http://pjp.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ypf.zdbjq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kbm.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jmt.nwbrower.top

TS:   s.slice(1, 4)
来源：http://cco.epnwcf.com

Java: s.substring(1, 4)
来源：http://oct.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://why.jqgfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://ved.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://iva.shzxlz.cn

[E04] 查找子串位置
来源：http://uqy.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://amg.wangdashe.top

PHP:  strpos($s, "x");
来源：http://wef.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://elj.cheryme.top

TS:   s.indexOf("x")
来源：http://vgs.dashuyun.cn

Java: s.indexOf("x")
来源：http://hmr.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://kcy.gotoacloud.top

Ruby: s.index("x")
来源：http://enn.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://lkg.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zht.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hov.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wvk.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ban.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://asa.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vso.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ofi.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kkh.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mhl.jlsjyb.cn

[E06] 替换子串
来源：http://phd.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tan.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://npi.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ljz.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://xfa.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kfr.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qre.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wgn.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://gam.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://abz.gotoacloud.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pqo.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sji.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ffc.nanxinkj.top

TS:   s.split(",")
来源：http://klr.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qki.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uzr.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://dmg.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xoj.vehdjk.com

[E08] 数组按分隔符合并
来源：http://ggj.tarul.cn

Py:   ",".join(items)
来源：http://uzp.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://png.zdbjq.cn

JS:   items.join(",")
来源：http://zjc.jqgufenzy.top

TS:   items.join(",")
来源：http://vio.sysykeji.top

Java: String.join(",", items)
来源：http://fvx.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://nvo.redwolf501.top

Ruby: items.join(",")
来源：http://jns.daria6918.cn

C#:   string.Join(",", items)
来源：http://eid.jqgfzy.top

[E09] 去除所有空白字符
来源：http://vzm.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sij.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ahk.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://jdq.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://ipy.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://leo.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://evp.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://udi.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wzj.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://rkl.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ebq.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kvc.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://fze.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://ctp.mhx1999.top

Java: String.format("%03d", 7)
来源：http://lqh.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://nsa.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tso.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ink.jinqigufen.top

[E11] 反转字符串
来源：http://fbp.shangyingyoupin.top

Py:   s[::-1]
来源：http://lju.zhixingplan.top

PHP:  strrev($s);
来源：http://pmy.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://ogk.yj202588.top

TS:   [...s].reverse().join("")
来源：http://akm.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ibv.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jrw.mhx1999.top

Ruby: s.reverse
来源：http://wfp.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qhs.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://bek.havefunace.top

Py:   s.count("a")
来源：http://xxu.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://knj.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://qby.sjlbkw.cn

TS:   s.split("a").length - 1
来源：http://ufu.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://her.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://bwf.yfazqb.com

Ruby: s.count("a")
来源：http://fco.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://arp.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://sob.316326.xyz

Py:   for ch in s: print(ch)
来源：http://sbs.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ebb.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gul.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wdn.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kjr.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://law.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://dxj.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zgo.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://sye.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qov.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eew.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://exa.xylfe.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cmg.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jjm.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://leg.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://soh.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cef.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://wle.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mnh.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gyz.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rkt.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mto.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oci.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mng.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://odo.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lcg.yfazqb.com

[E16] 数字千分位
来源：http://jra.yj20258.top

Py:   f"{1234567:,}"
来源：http://zne.aizwys.cn

PHP:  number_format(1234567);
来源：http://asq.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mkb.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hni.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sng.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mws.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qew.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://nbq.jinqigufen.top

[E17] 首字母大写
来源：http://mwx.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ekb.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ldt.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://imk.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://brq.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ggd.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fjr.yj20258888.top

Ruby: s.capitalize
来源：http://eck.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dqg.dashuyun.cn

[E18] 模板占位符替换
来源：http://siu.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wqd.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kjl.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vtl.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ymz.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hxg.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gon.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dnp.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wfx.daria6918.cn

[E19] 多行文本按行拆分
来源：http://omp.yanxiufei.cn

Py:   s.splitlines()
来源：http://uwi.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fng.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://enz.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://viq.fehbvm.com

Java: s.lines().toList()
来源：http://wtz.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://ica.wangdashe.top

Ruby: s.lines
来源：http://gsr.zdqjudy.top

C#:   s.Split('\n')
来源：http://fto.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://eww.xuanzx.com

Py:   if not s:
来源：http://jim.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tih.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fmx.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://lfs.sxryk.cn

Java: if (s.isEmpty()) {}
来源：http://fbt.ydjk.org.cn

Go:   if s == "" {}
来源：http://hpf.sxryk.cn

Ruby: if s.empty?
来源：http://sau.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vtt.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://wkp.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wtn.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ntl.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ivx.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tzw.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fif.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://mpm.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ndi.zhengqikj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://llk.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://idc.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ttx.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://poh.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://koo.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cwi.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rvg.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yvk.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://xfa.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xxv.0kj1m.cn

================================================================================
来源：http://qdw.zdqjudy.top

F. 文件与目录
来源：http://uyk.guannengcc.top

================================================================================
来源：http://khj.tarul.cn

[F01] 读取整个文件
来源：http://vlc.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rev.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://agi.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tve.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cra.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wsb.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dxt.daxiang520.top

Ruby: File.read("a.txt")
来源：http://isa.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://djx.c1oappe.top

[F02] 逐行读取文件
来源：http://btj.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://npp.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hxf.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qnc.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eqe.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://glx.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://khb.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zbj.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zyk.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://ndi.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://exj.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hee.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://smz.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hac.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kue.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ipa.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://hvb.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rvv.gaohongyu789.top

[F04] 追加写入文件
来源：http://yvp.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qtf.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vck.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fpr.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://igu.jianghu66.top


<!-- 参考信息 -->