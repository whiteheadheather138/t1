代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hyw.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ihs.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://xoe.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://zbw.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://edb.cashguo.top

[D20] 统计每个元素出现次数
来源：http://ziw.zhiwuduotai.top

Py:   Counter(arr)
来源：http://hdc.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://gry.shangyingyoupin.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://llz.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gat.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://slo.cdnleiting.top

Go:   // 手写 map[T]int
来源：http://etu.chenlongwang.top

Ruby: arr.tally
来源：http://wjj.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jzz.chenlongwang.top

[D21] 判断是否包含某元素
来源：http://lzu.gzhubu.top

Py:   x in arr
来源：http://zcd.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://vaw.smart0.xyz

JS:   arr.includes(x)
来源：http://agv.zhongyouzk.top

TS:   arr.includes(x)
来源：http://qcy.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://pzk.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://ivv.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://wng.zhijiandao.cn

C#:   list.Contains(x)
来源：http://kcm.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://qsk.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fpb.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uln.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bpn.hysaishi.cn

TS:   [...arr];
来源：http://zxu.sysykeji.top

Java: new ArrayList<>(list);
来源：http://rov.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://kad.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://qjy.hammf.cn

C#:   new List<int>(list);
来源：http://emd.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://mqb.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wzd.yj202588.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tku.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hyc.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cwu.tianlin.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://pxa.jiagoushi.top

Go:   // 手写循环
来源：http://wrn.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pnp.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jkp.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://dvv.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fpm.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gjx.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://onl.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://muk.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mxe.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sjm.gogol.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qyz.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://izk.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://dof.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xst.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oer.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ilo.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://avo.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lpb.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://omz.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://frs.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vrv.cqqwz.cn

[D26] 数组转字符串
来源：http://wmm.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://rwp.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://yiu.ydzc1.top

JS:   arr.join(", ")
来源：http://nej.bjfxy.top

TS:   arr.join(", ")
来源：http://jkv.aibaodan.cn

Java: String.join(", ", list)
来源：http://vww.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://bfv.shzxlz.cn

Ruby: arr.join(", ")
来源：http://ypn.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://rhs.hnxiangtu.top

================================================================================
来源：http://jhq.xuanzx.com

E. 字符串处理
来源：http://kex.meibo888.top

================================================================================
来源：http://fxu.nwbrower.top

[E01] 拼接字符串
来源：http://did.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jxz.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ind.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qcx.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rfl.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pmv.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dhc.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pkh.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qmj.bjfxy.top

[E02] 重复字符串
来源：http://lds.xinyue.icu

Py:   "ab" * 3
来源：http://nlv.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://sbu.sxryk.cn

JS:   "ab".repeat(3)
来源：http://jnb.yonumen.top

TS:   "ab".repeat(3)
来源：http://rki.snrcjt.cn

Java: "ab".repeat(3)
来源：http://kcs.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://rdy.tarul.cn

Ruby: "ab" * 3
来源：http://tlh.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nkl.guowangkeji.top

[E03] 截取子串
来源：http://tvq.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dat.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://thq.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gag.meibo888.top

TS:   s.slice(1, 4)
来源：http://wsk.ybcxt.top

Java: s.substring(1, 4)
来源：http://ytp.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lmp.zycfv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lio.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://joj.zhiwuduotai.top

[E04] 查找子串位置
来源：http://wez.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://dba.fktsv.cn

PHP:  strpos($s, "x");
来源：http://ooj.shanyushiyangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://erk.shuidangran.top

TS:   s.indexOf("x")
来源：http://rcb.tanke756.top

Java: s.indexOf("x")
来源：http://zzb.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://eof.sjlbkw.cn

Ruby: s.index("x")
来源：http://rjx.fengsongda.top

C#:   s.IndexOf("x")
来源：http://mdf.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kjm.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ngh.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hsy.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cav.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://kbi.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yzu.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gna.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://itw.nanxuanxn.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nhm.andypj.xyz

[E06] 替换子串
来源：http://uli.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sdj.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://lqu.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zqv.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://noo.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xum.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ukf.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://apd.yonumen.top

C#:   s.Replace("a", "b")
来源：http://aih.dianchejie.cn

[E07] 按分隔符拆分
来源：http://yqd.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tgn.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sdz.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://atg.nanxinkj.top

TS:   s.split(",")
来源：http://zol.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://dde.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ogg.tanke756.top

Ruby: s.split(",");  s.split
来源：http://bxb.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fkv.hammf.cn

[E08] 数组按分隔符合并
来源：http://dgg.zhoulong.xyz

Py:   ",".join(items)
来源：http://kdx.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://bdm.ctjpmb.com

JS:   items.join(",")
来源：http://lep.ppjwa.cn

TS:   items.join(",")
来源：http://kme.hcnkem.com

Java: String.join(",", items)
来源：http://pux.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://dkr.shzxlz.cn

Ruby: items.join(",")
来源：http://ihb.yj20258888.top

C#:   string.Join(",", items)
来源：http://ymb.chenlongwang.top

[E09] 去除所有空白字符
来源：http://apz.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ubr.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tkj.zhengqikj.top

JS:   s.replace(/\s+/g, "")
来源：http://cgz.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://wyl.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://cjg.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://kuk.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ora.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://doh.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://khp.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://plk.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bmn.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://mgc.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://loy.shzxlz.cn

Java: String.format("%03d", 7)
来源：http://ewa.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://mpx.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ima.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jxu.tarul.cn

[E11] 反转字符串
来源：http://nzm.sxryk.cn

Py:   s[::-1]
来源：http://vxd.chenzaomai.com

PHP:  strrev($s);
来源：http://uiy.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://hym.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://sgk.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://pqf.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://imr.fanxiaobao.xyz

Ruby: s.reverse
来源：http://pdw.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pbw.fehbvm.com

[E12] 统计某字符出现次数
来源：http://wed.redwolf501.top

Py:   s.count("a")
来源：http://slw.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://uun.yj20258.top

JS:   s.split("a").length - 1
来源：http://mtq.hnqzz.top

TS:   s.split("a").length - 1
来源：http://ygs.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ykt.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://lgh.hongshengwenyu.top

Ruby: s.count("a")
来源：http://mya.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://ssz.fanxiaobao.xyz

[E13] 逐字符遍历
来源：http://zhi.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://uwk.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://atq.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jwa.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://apv.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mes.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rhd.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sjt.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ohj.meibo888.top

[E14] URL 编码与 Base64
来源：http://tef.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qpx.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zbk.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uvc.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://elq.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://esn.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vff.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bgm.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://shl.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://exk.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tje.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hwn.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qdn.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cwh.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mnv.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cji.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aqt.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dcw.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://pid.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://thn.yj20258.top

PHP:  number_format(1234567);
来源：http://gtd.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hey.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://imo.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yqv.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tvr.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ozl.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://gyb.mhx1999.top

[E17] 首字母大写
来源：http://onn.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vqr.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yff.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://itb.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pjy.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uvp.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nez.zhixingplan.top

Ruby: s.capitalize
来源：http://ncc.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wkn.zhixingplan.top

[E18] 模板占位符替换
来源：http://ymy.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xpq.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eix.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ufu.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://shg.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gjs.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bkr.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://omc.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xdc.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://dng.kuanghao11.cn

Py:   s.splitlines()
来源：http://hdf.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bne.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://ajw.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://phr.epnwcf.com

Java: s.lines().toList()
来源：http://hwe.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://oip.ivvv.top

Ruby: s.lines
来源：http://cna.9152youxi.cn

C#:   s.Split('\n')
来源：http://yum.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://fta.yfazqb.com

Py:   if not s:
来源：http://txe.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pji.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gil.kuanghao11.cn

TS:   if (s === "") {}
来源：http://dmo.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://mqs.zhixingplan.top

Go:   if s == "" {}
来源：http://yfz.ehwqpu.com

Ruby: if s.empty?
来源：http://los.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dpk.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://lun.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://saj.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://egv.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://byx.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ukl.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://knn.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://fcr.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://frp.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vcw.jianghu66.top

[E22] 字节长度与字符长度
来源：http://ksb.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ooq.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nwe.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://swg.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://alu.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xjo.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zea.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://zvj.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wmg.wangdashe.top

================================================================================
来源：http://mvy.haohaochexian.top

F. 文件与目录
来源：http://uvb.nanxinkj.top

================================================================================
来源：http://cmx.redwolf501.top

[F01] 读取整个文件
来源：http://dyo.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zaw.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://dzc.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cwl.cqqwz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://neq.zhoulong.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://wkd.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://upg.hcnkem.com

Ruby: File.read("a.txt")
来源：http://feh.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://oxg.dianchejie.cn

[F02] 逐行读取文件
来源：http://esw.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nks.zhengqikj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://omu.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zdn.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fwf.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bso.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xqj.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://taf.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://syy.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://ved.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aii.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qge.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uck.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sux.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wyi.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ydd.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://xve.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ikb.zhijiandao.cn

[F04] 追加写入文件
来源：http://nvk.gogol.net.cn


<!-- 参考信息 -->