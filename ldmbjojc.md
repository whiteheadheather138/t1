代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://azc.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lop.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hbz.shuidangran.top

Go:   // 手写 map[T]int
来源：http://hrh.zhengqikj.top

Ruby: arr.tally
来源：http://pzv.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://exv.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://iei.fktsv.cn

Py:   x in arr
来源：http://flu.chenjidiqi.icu

PHP:  in_array($x, $arr, true);
来源：http://lce.yongpay.top

JS:   arr.includes(x)
来源：http://pmj.quarkkingdee.top

TS:   arr.includes(x)
来源：http://pzx.52xcode.cn

Java: list.contains(x)
来源：http://dwe.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://poy.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://rmu.ydzc1.top

C#:   list.Contains(x)
来源：http://aux.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://vev.nanxuanxn.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hhb.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nin.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ssa.andypj.xyz

TS:   [...arr];
来源：http://llq.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://jen.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://hky.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://iwp.zdqjudy.top

C#:   new List<int>(list);
来源：http://maq.jqgfzy.top

[D23] reduce 累积计算
来源：http://bpr.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xgn.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qjm.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jkh.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zjx.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fzb.cheryme.top

Go:   // 手写循环
来源：http://nro.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gts.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://scx.0kj1m.cn

[D24] 字典 / Map 基本操作
来源：http://rgt.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://spt.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mgb.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://asw.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://anc.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bdt.ydjk.org.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oye.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hqz.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jjc.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://fvt.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eqr.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cph.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fgp.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xul.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iwn.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kvd.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cwf.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://riq.yfazqb.com

[D26] 数组转字符串
来源：http://von.bbcook.cn

Py:   ", ".join(map(str, arr))
来源：http://mdi.yonumen.top

PHP:  implode(", ", $arr);
来源：http://mlf.hywenlv.cn

JS:   arr.join(", ")
来源：http://jcn.ydzc1.top

TS:   arr.join(", ")
来源：http://tqn.yj20258.top

Java: String.join(", ", list)
来源：http://zlm.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://lfx.dashuyun.cn

Ruby: arr.join(", ")
来源：http://qdd.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://rmk.gogol.net.cn

================================================================================
来源：http://dlv.fktsv.cn

E. 字符串处理
来源：http://kcd.meibo888.top

================================================================================
来源：http://lhc.yonumen.top

[E01] 拼接字符串
来源：http://fhb.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dzt.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aui.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uwl.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yng.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://etr.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gjs.nwbrower.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jqg.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zne.fehbvm.com

[E02] 重复字符串
来源：http://suy.guowangkeji.top

Py:   "ab" * 3
来源：http://vjh.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://hks.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://ehu.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://cko.xuanzx.com

Java: "ab".repeat(3)
来源：http://ite.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://yez.ydzc1.top

Ruby: "ab" * 3
来源：http://knk.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nen.yueranfly.top

[E03] 截取子串
来源：http://oks.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ffa.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gyx.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fpo.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://cpc.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://tlc.ywan-chungtsiang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tjm.0kj1m.cn

Ruby: s[1, 3];  s[1..3]
来源：http://klp.meibo888.top

C#:   s.Substring(1, 3)
来源：http://kwq.fengsongda.top

[E04] 查找子串位置
来源：http://knd.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://eog.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://ywq.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jco.wangdashe.top

TS:   s.indexOf("x")
来源：http://xqf.hnxiangtu.top

Java: s.indexOf("x")
来源：http://dhy.ivvv.top

Go:   strings.Index(s, "x")
来源：http://tuz.mhx1999.top

Ruby: s.index("x")
来源：http://cjh.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://xrw.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ome.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nue.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eef.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hnf.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qve.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nml.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://des.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wsa.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fzg.pycfn.com

[E06] 替换子串
来源：http://vfi.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lea.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://snb.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://avz.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://ngn.9152youxi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zhn.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ndh.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://grs.cashguo.top

C#:   s.Replace("a", "b")
来源：http://bcd.yuanzhike.top

[E07] 按分隔符拆分
来源：http://qla.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://znz.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://osp.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gwi.shuidangran.top

TS:   s.split(",")
来源：http://gzl.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://cej.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oyu.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://ugh.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://suh.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://xhn.zycfv.cn

Py:   ",".join(items)
来源：http://hgq.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://qay.gaohongyu789.top

JS:   items.join(",")
来源：http://tdq.cheryme.top

TS:   items.join(",")
来源：http://nkc.epnwcf.com

Java: String.join(",", items)
来源：http://oft.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://por.ydjk.org.cn

Ruby: items.join(",")
来源：http://stp.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://xzb.shuidangran.top

[E09] 去除所有空白字符
来源：http://eqk.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tdu.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ygj.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://ucu.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://cnl.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://bgf.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hra.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ldr.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jmx.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://bii.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nmn.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://afe.zhongyouzk.top

JS:   "7".padStart(3, "0")
来源：http://okx.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://vyg.sweek.top

Java: String.format("%03d", 7)
来源：http://dka.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://dtt.svipenyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ylz.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uhq.fengsongda.top

[E11] 反转字符串
来源：http://ekw.xinyue.icu

Py:   s[::-1]
来源：http://zgl.nanxuanxn.top

PHP:  strrev($s);
来源：http://jkk.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://yju.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://jmx.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vya.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jst.jinqigfzy.top

Ruby: s.reverse
来源：http://cvc.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://saw.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://zkv.yueranfly.top

Py:   s.count("a")
来源：http://mqa.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://cwa.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://zew.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://kvf.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tcj.tanke756.top

Go:   strings.Count(s, "a")
来源：http://otg.yueranfly.top

Ruby: s.count("a")
来源：http://ckl.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://lht.yuxming.cn

[E13] 逐字符遍历
来源：http://icl.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://rjz.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yto.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vcr.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mbp.uphjek.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fpi.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vbq.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iel.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://awj.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://ege.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lkl.smart0.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://wrs.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fdv.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qav.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rzs.sufxvd.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xar.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qrf.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pex.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://bwa.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cgs.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nas.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pta.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ypk.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pwl.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wtc.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bps.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jtm.jinghuilouyu.cn

[E16] 数字千分位
来源：http://tsa.andypj.xyz

Py:   f"{1234567:,}"
来源：http://qjz.hammf.cn

PHP:  number_format(1234567);
来源：http://oye.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://soc.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cnz.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://thq.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://git.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://had.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://tsn.jiagoushi.top

[E17] 首字母大写
来源：http://civ.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tak.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fmq.jinghuilouyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oac.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ilu.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zos.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sie.vqdsnc.cn

Ruby: s.capitalize
来源：http://sio.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hmw.ydjk.org.cn

[E18] 模板占位符替换
来源：http://wxz.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://scs.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://glh.xziqi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wke.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qeg.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jen.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://odd.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bnz.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://phj.tanke756.top

[E19] 多行文本按行拆分
来源：http://ddi.sxryk.cn

Py:   s.splitlines()
来源：http://tta.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qju.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://fnn.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://xse.smart0.xyz

Java: s.lines().toList()
来源：http://fjp.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://qki.yvedp.cn

Ruby: s.lines
来源：http://qri.guannengcc.top

C#:   s.Split('\n')
来源：http://jdo.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://pgi.epnwcf.com

Py:   if not s:
来源：http://kgl.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://njv.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://luh.nwbrower.top

TS:   if (s === "") {}
来源：http://cpr.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://ckz.andypj.xyz

Go:   if s == "" {}
来源：http://coj.ehwqpu.com

Ruby: if s.empty?
来源：http://hat.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dft.ehwqpu.com

[E21] 超长截断加省略号
来源：http://bwb.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vdk.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rto.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yme.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://suy.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lxk.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://kjb.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bmp.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jkd.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://aus.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://coo.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fic.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hdu.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ywx.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qbc.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uix.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://uwn.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hgn.hongshengwenyu.top

================================================================================
来源：http://xqo.zhaomingkeji.xyz

F. 文件与目录
来源：http://nzv.jqgufenzy.top

================================================================================
来源：http://sfe.c1oappe.top

[F01] 读取整个文件
来源：http://uap.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kxe.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://ram.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://obf.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://riv.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sgh.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iaz.cheryme.top

Ruby: File.read("a.txt")
来源：http://nsx.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://agb.zhijiandao.cn

[F02] 逐行读取文件
来源：http://tuz.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mvo.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rfi.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nvt.feifeiyinyue.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cvb.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uzr.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bii.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xdp.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xbk.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://qme.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rhf.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ypv.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://voj.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pag.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yxf.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://awd.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://toi.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://whg.iojbl.cn

[F04] 追加写入文件
来源：http://kxi.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qvw.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://isz.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bnh.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nsw.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kcf.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yju.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://chs.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rio.meibo888.top


<!-- 参考信息 -->