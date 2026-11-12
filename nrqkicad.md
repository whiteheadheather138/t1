代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://umg.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xby.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://ltm.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rvk.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eur.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://foe.52xcode.cn

Py:   Counter(arr)
来源：http://wcw.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://but.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bot.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uay.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://beu.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://fze.jiagoushi.top

Ruby: arr.tally
来源：http://tiy.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yeh.wangdashe.top

[D21] 判断是否包含某元素
来源：http://xrw.yfazqb.com

Py:   x in arr
来源：http://ack.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://whv.cashguo.top

JS:   arr.includes(x)
来源：http://gyu.tianlin.xyz

TS:   arr.includes(x)
来源：http://cum.bbcook.cn

Java: list.contains(x)
来源：http://maq.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://fmg.shzxlz.cn

Ruby: arr.include?(x)
来源：http://nyb.gogol.net.cn

C#:   list.Contains(x)
来源：http://gff.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://eso.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vcc.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://asi.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yex.xylfe.cn

TS:   [...arr];
来源：http://kyv.cashguo.top

Java: new ArrayList<>(list);
来源：http://mfw.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qbx.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://xte.yfazqb.com

C#:   new List<int>(list);
来源：http://xxg.iojbl.cn

[D23] reduce 累积计算
来源：http://qvt.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wvt.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://owp.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dnw.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hvo.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rqb.tanke756.top

Go:   // 手写循环
来源：http://asb.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://klb.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qof.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://cvt.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jns.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ffx.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://szl.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pvh.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vkw.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zpz.yonumen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ryo.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sib.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://kkm.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://abn.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cov.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dqk.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://klh.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nrq.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mkz.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ioj.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://foh.zhongyouzk.top

[D26] 数组转字符串
来源：http://bqb.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://krt.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://cix.hfpthk.cn

JS:   arr.join(", ")
来源：http://apw.hcnkem.com

TS:   arr.join(", ")
来源：http://kuo.cheryme.top

Java: String.join(", ", list)
来源：http://fwg.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://nch.birdmap.top

Ruby: arr.join(", ")
来源：http://laq.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://crx.yuxming.cn

================================================================================
来源：http://uut.feifeiyinyue.top

E. 字符串处理
来源：http://xhb.daxiang520.top

================================================================================
来源：http://nde.yuanzhike.top

[E01] 拼接字符串
来源：http://gjc.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ejb.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zwt.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kxj.wangshuangyany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jxp.c1oappe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mni.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vta.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vqm.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://age.daria6918.cn

[E02] 重复字符串
来源：http://yly.jyoumei.cn

Py:   "ab" * 3
来源：http://wha.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://mip.yongpay.top

JS:   "ab".repeat(3)
来源：http://hzk.smart0.xyz

TS:   "ab".repeat(3)
来源：http://lkf.daxiang520.top

Java: "ab".repeat(3)
来源：http://wvf.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://nhz.epnwcf.com

Ruby: "ab" * 3
来源：http://vps.316326.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lih.yuxming.cn

[E03] 截取子串
来源：http://ssf.quarkkingdee.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cmg.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bwy.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://imz.yvedp.cn

TS:   s.slice(1, 4)
来源：http://cpj.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://fwc.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://elx.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://qyr.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://ktb.wangdashe.top

[E04] 查找子串位置
来源：http://tqp.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://zik.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://ifs.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sou.zycfv.cn

TS:   s.indexOf("x")
来源：http://nvl.ybcxt.top

Java: s.indexOf("x")
来源：http://lov.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://yne.wangshuangyany.cn

Ruby: s.index("x")
来源：http://cxa.xziqi.cn

C#:   s.IndexOf("x")
来源：http://cpx.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zch.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nli.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qsf.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jid.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://hjd.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://syz.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xnd.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eea.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dff.hywenlv.cn

[E06] 替换子串
来源：http://mrh.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dbo.tianlin.xyz

PHP:  str_replace("a", "b", $s);
来源：http://wei.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ywz.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://gme.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://klt.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lts.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sxn.yj202588.top

C#:   s.Replace("a", "b")
来源：http://mso.snrcjt.cn

[E07] 按分隔符拆分
来源：http://zwy.pengpengdd.cyou

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qyw.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pwy.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vfx.chenlongwang.top

TS:   s.split(",")
来源：http://byc.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wzi.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yhw.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://ghp.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://but.fengsongda.top

[E08] 数组按分隔符合并
来源：http://pev.zhongyouzk.top

Py:   ",".join(items)
来源：http://dgu.snrcjt.cn

PHP:  implode(",", $items);
来源：http://pxh.wangdashe.top

JS:   items.join(",")
来源：http://ueb.vehdjk.com

TS:   items.join(",")
来源：http://cmw.jinqigufen.top

Java: String.join(",", items)
来源：http://lnp.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://xqp.yj20258.top

Ruby: items.join(",")
来源：http://rdu.yfazqb.com

C#:   string.Join(",", items)
来源：http://pff.epnwcf.com

[E09] 去除所有空白字符
来源：http://epw.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ybe.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zix.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://tco.tianlin.xyz

TS:   s.replace(/\s+/g, "")
来源：http://hbt.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://hso.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jwl.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://ntg.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fcg.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://ibs.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zmu.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://krk.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://aat.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://pyl.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://rkc.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://yrx.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wph.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kue.sufxvd.cn

[E11] 反转字符串
来源：http://wom.zhongyouzk.top

Py:   s[::-1]
来源：http://hfs.chenlongwang.top

PHP:  strrev($s);
来源：http://pwn.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://ykx.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://sdl.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://znx.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://rem.tanke756.top

Ruby: s.reverse
来源：http://hpo.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://gwg.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://xuq.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://cys.316326.xyz

PHP:  substr_count($s, "a");
来源：http://isc.redwolf501.top

JS:   s.split("a").length - 1
来源：http://lew.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://fpw.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lsf.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://jgy.gotoacloud.top

Ruby: s.count("a")
来源：http://icd.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://bgr.hywenlv.cn

[E13] 逐字符遍历
来源：http://wdx.ivvv.top

Py:   for ch in s: print(ch)
来源：http://vae.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jhg.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iaw.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lpm.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xsn.zhongyouzk.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://srr.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kis.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ixe.aizwys.cn

[E14] URL 编码与 Base64
来源：http://epq.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iio.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kvf.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yna.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://swc.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wis.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://glq.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wbj.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ubb.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://pyv.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mih.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kcd.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vdy.ppjwa.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jdu.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fsu.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qeo.hammf.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tyn.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cdd.cqqwz.cn

[E16] 数字千分位
来源：http://agj.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://omm.jqgfzy.top

PHP:  number_format(1234567);
来源：http://cua.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://teu.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gwf.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://efj.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://slu.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qkd.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://ocz.zycfv.cn

[E17] 首字母大写
来源：http://qsl.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tng.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vdv.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lah.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://adf.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gyq.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://byb.epnwcf.com

Ruby: s.capitalize
来源：http://nhu.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lxk.cqqwz.cn

[E18] 模板占位符替换
来源：http://zpz.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uli.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xay.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tqo.pengpengdd.cyou

TS:   tpl.replaceAll("{name}", name)
来源：http://ixx.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bzx.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vnp.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vsk.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aed.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://ynn.tianlin.xyz

Py:   s.splitlines()
来源：http://bsx.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gnu.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://oop.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://weo.jinqigufen.top

Java: s.lines().toList()
来源：http://pcr.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://jbk.yueranfly.top

Ruby: s.lines
来源：http://qir.0kj1m.cn

C#:   s.Split('\n')
来源：http://jvz.nwbrower.top

[E20] 判断字符串是否为空
来源：http://ddw.nanxinkj.top

Py:   if not s:
来源：http://que.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rdi.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lfc.shuidangran.top

TS:   if (s === "") {}
来源：http://htv.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://swg.cdnleiting.top

Go:   if s == "" {}
来源：http://usa.cdnleiting.top

Ruby: if s.empty?
来源：http://kcr.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sqw.316326.xyz

[E21] 超长截断加省略号
来源：http://obs.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ehs.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wfi.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://api.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zqe.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bjv.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://yrj.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://odk.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://spr.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://eub.redwolf501.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pby.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ziq.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bnv.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hvt.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tjh.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lgn.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://yky.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nqy.xingfuxueyuan.xyz

================================================================================
来源：http://pim.yuanzhike.top

F. 文件与目录
来源：http://opn.dashuyun.cn

================================================================================
来源：http://uej.yonumen.top

[F01] 读取整个文件
来源：http://zgf.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xmf.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://tjd.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ush.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://obi.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://npx.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nez.tarul.cn

Ruby: File.read("a.txt")
来源：http://mff.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://jfx.nanxuanxn.top

[F02] 逐行读取文件
来源：http://hvu.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ouj.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://smk.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yeh.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rjy.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ugu.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qnq.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zgo.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://urk.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://hpx.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ghh.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://pxi.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fvb.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ylz.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dzp.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uug.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://anz.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sgz.chenjidiqi.icu

[F04] 追加写入文件
来源：http://gmq.epnwcf.com


<!-- 参考信息 -->