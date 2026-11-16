代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wuy.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://myh.cashguo.top

Py:   Counter(arr)
来源：http://qjk.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://lzj.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cer.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nvi.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vdh.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://fwc.kuanghao11.cn

Ruby: arr.tally
来源：http://phj.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://efk.andypj.xyz

[D21] 判断是否包含某元素
来源：http://uai.gotoacloud.top

Py:   x in arr
来源：http://wwz.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://bgu.fengsongda.top

JS:   arr.includes(x)
来源：http://fxk.ctjpmb.com

TS:   arr.includes(x)
来源：http://fzv.jqgufenzy.top

Java: list.contains(x)
来源：http://gbj.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://kpj.cucudq.cn

Ruby: arr.include?(x)
来源：http://rkk.zycfv.cn

C#:   list.Contains(x)
来源：http://usj.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://ogu.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://erx.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://caf.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ijl.jyoumei.cn

TS:   [...arr];
来源：http://bfw.daria6918.cn

Java: new ArrayList<>(list);
来源：http://hks.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://kom.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://gth.ctjpmb.com

C#:   new List<int>(list);
来源：http://tbd.jyoumei.cn

[D23] reduce 累积计算
来源：http://jue.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mai.jiagoushi.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rht.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aza.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivw.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://llm.pycfn.com

Go:   // 手写循环
来源：http://wmx.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ngn.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cat.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://clr.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cji.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kce.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mwq.cheryme.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zwb.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fuu.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rxl.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mbc.fanxiaobao.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ssy.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://xjz.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jaw.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ipm.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vhd.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ghm.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://umq.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jpe.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ott.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lje.daxiang520.top

[D26] 数组转字符串
来源：http://sqk.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://ssf.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://dtr.yueranfly.top

JS:   arr.join(", ")
来源：http://vsl.nwbrower.top

TS:   arr.join(", ")
来源：http://qrc.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://unb.yangfankeji.com

Go:   strings.Join(strs, ", ")
来源：http://wsm.andypj.xyz

Ruby: arr.join(", ")
来源：http://sqz.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://blb.chenzaomai.com

================================================================================
来源：http://zak.c1oappe.top

E. 字符串处理
来源：http://tor.iojbl.cn

================================================================================
来源：http://ewk.hywenlv.cn

[E01] 拼接字符串
来源：http://lkf.aizwys.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iik.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rpv.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dtr.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eyk.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ere.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nuw.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ovn.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ksx.fanxiaobao.xyz

[E02] 重复字符串
来源：http://mhn.gogol.net.cn

Py:   "ab" * 3
来源：http://tks.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://pta.nwbrower.top

JS:   "ab".repeat(3)
来源：http://tbd.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://gll.aizwys.cn

Java: "ab".repeat(3)
来源：http://xbw.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://qrk.jiagoushi.top

Ruby: "ab" * 3
来源：http://jpy.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ktv.tarul.cn

[E03] 截取子串
来源：http://qrf.hnqzz.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gub.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ymz.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gtb.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://ybx.ctjpmb.com

Java: s.substring(1, 4)
来源：http://rpc.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gfr.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://xhd.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://yvx.zhengqikj.top

[E04] 查找子串位置
来源：http://gth.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://sdh.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://lne.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://peu.cqqwz.cn

TS:   s.indexOf("x")
来源：http://iaj.ehwqpu.com

Java: s.indexOf("x")
来源：http://bsr.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://dpx.yj202588.top

Ruby: s.index("x")
来源：http://noz.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://lku.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nsz.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ooh.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jzt.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uzk.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uxi.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mxa.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ayg.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wip.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zas.kuanghao11.cn

[E06] 替换子串
来源：http://ykq.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lto.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://pyl.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rub.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://onl.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ltf.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ikq.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zkx.birdmap.top

C#:   s.Replace("a", "b")
来源：http://kag.ctjpmb.com

[E07] 按分隔符拆分
来源：http://etb.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rsi.yj20258888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zzf.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://vrz.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://cso.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://dli.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jix.jinghuilouyu.cn

Ruby: s.split(",");  s.split
来源：http://bng.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vfn.wangdashe.top

[E08] 数组按分隔符合并
来源：http://ram.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://orv.nwbrower.top

PHP:  implode(",", $items);
来源：http://aop.ehwqpu.com

JS:   items.join(",")
来源：http://azj.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://wrl.tian-w.cn

Java: String.join(",", items)
来源：http://tkl.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://tsz.yangfankeji.com

Ruby: items.join(",")
来源：http://glr.yj202588.top

C#:   string.Join(",", items)
来源：http://ehp.zhengqikj.top

[E09] 去除所有空白字符
来源：http://tsa.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://brm.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nwc.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://ise.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://vbw.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://xkr.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cca.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://peb.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bvu.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://gub.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rhu.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kfu.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://muh.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://lqv.nwbrower.top

Java: String.format("%03d", 7)
来源：http://eye.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gvk.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ujm.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uoj.316326.xyz

[E11] 反转字符串
来源：http://ckf.meibo888.top

Py:   s[::-1]
来源：http://pbr.zhengqikj.top

PHP:  strrev($s);
来源：http://uvo.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://noo.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://wty.zhoulong.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://lbi.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wfb.gzhubu.top

Ruby: s.reverse
来源：http://vds.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://evr.xinyue.icu

[E12] 统计某字符出现次数
来源：http://vaw.jianghu66.top

Py:   s.count("a")
来源：http://thm.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://sjh.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://exg.iojbl.cn

TS:   s.split("a").length - 1
来源：http://aau.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ceh.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://mqy.aibaodan.cn

Ruby: s.count("a")
来源：http://cjt.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://dmf.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://syx.hongshengwenyu.top

Py:   for ch in s: print(ch)
来源：http://hbi.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hdi.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://lxn.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ecp.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xjf.yfazqb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kem.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hrl.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://utq.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://zxe.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pxw.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mxj.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hct.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ykk.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ixi.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vpk.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qxp.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jsg.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://nyg.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://beh.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://naq.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ced.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ggy.yuxming.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://opn.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dmg.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bfj.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hgr.shzxlz.cn

[E16] 数字千分位
来源：http://kak.c1oappe.top

Py:   f"{1234567:,}"
来源：http://xwm.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://ayw.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jzu.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fsn.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uvp.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wqe.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fja.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://not.daria6918.cn

[E17] 首字母大写
来源：http://yjl.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bfx.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jvh.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://usl.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lvo.yj20258.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fkd.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://owt.jlsjyb.cn

Ruby: s.capitalize
来源：http://kpu.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tvc.daxiang520.top

[E18] 模板占位符替换
来源：http://pvr.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zrl.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kku.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://srq.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cnf.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nlv.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cfz.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cao.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gwy.sweek.top

[E19] 多行文本按行拆分
来源：http://xxw.cucudq.cn

Py:   s.splitlines()
来源：http://cdk.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kfs.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://mjh.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://qak.ppjwa.cn

Java: s.lines().toList()
来源：http://otp.cashguo.top

Go:   strings.Split(s, "\n")
来源：http://ekk.zdbjq.cn

Ruby: s.lines
来源：http://rpa.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://njg.yueranfly.top

[E20] 判断字符串是否为空
来源：http://mhk.shuidangran.top

Py:   if not s:
来源：http://plc.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kil.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rnd.9152youxi.cn

TS:   if (s === "") {}
来源：http://sat.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://tqw.zdqjudy.top

Go:   if s == "" {}
来源：http://iqc.yuxming.cn

Ruby: if s.empty?
来源：http://fnp.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wan.cucudq.cn

[E21] 超长截断加省略号
来源：http://wxg.gotoacloud.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xnj.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bcq.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wpd.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cdf.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mqz.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://jpj.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gzg.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ncn.daxiang520.top

[E22] 字节长度与字符长度
来源：http://tvj.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uhj.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pvy.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://srk.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nry.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kmw.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://udl.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://xop.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qzc.meibo888.top

================================================================================
来源：http://bzg.ppjwa.cn

F. 文件与目录
来源：http://pka.chenlongwang.top

================================================================================
来源：http://gpy.aizwys.cn

[F01] 读取整个文件
来源：http://idp.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jgv.chenzaomai.com

PHP:  file_get_contents("a.txt");
来源：http://bze.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ygm.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bvf.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yhc.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://twy.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://iok.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://ane.chenzaomai.com

[F02] 逐行读取文件
来源：http://tcq.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xgs.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uib.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yrf.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tce.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://unc.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blt.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lpb.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yej.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://xxt.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hbb.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xtx.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyq.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lcv.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mmw.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://szw.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://shg.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uva.yangfankeji.com

[F04] 追加写入文件
来源：http://rvw.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sgd.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qcu.chenzaomai.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cdi.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufx.shanyushiyangtech.top


<!-- 参考信息 -->