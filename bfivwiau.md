代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://rca.shzxlz.cn

Ruby: arr.include?(x)
来源：http://sao.svipenyu.cn

C#:   list.Contains(x)
来源：http://flo.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://gie.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ctf.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gbu.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nan.yvedp.cn

TS:   [...arr];
来源：http://pzc.yongpay.top

Java: new ArrayList<>(list);
来源：http://eaa.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://zth.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://fmb.yueranfly.top

C#:   new List<int>(list);
来源：http://dpj.shzxlz.cn

[D23] reduce 累积计算
来源：http://iho.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uox.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vur.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://emy.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://piz.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xja.yuxming.cn

Go:   // 手写循环
来源：http://rav.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mgp.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qcw.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://hal.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gzb.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tll.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bbf.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wkc.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kgm.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sey.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qwq.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hbr.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://rbr.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yzc.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mqj.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vdd.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ere.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zry.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jck.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ntl.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ipt.jinqigfzy.top

[D26] 数组转字符串
来源：http://xna.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://hjv.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://wls.chenlongwang.top

JS:   arr.join(", ")
来源：http://gwy.yueranfly.top

TS:   arr.join(", ")
来源：http://bgb.sxryk.cn

Java: String.join(", ", list)
来源：http://ngt.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://hrw.yuanzhike.top

Ruby: arr.join(", ")
来源：http://vqv.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://qib.tarul.cn

================================================================================
来源：http://vay.jinqigfzy.top

E. 字符串处理
来源：http://dck.fanxiaobao.xyz

================================================================================
来源：http://clc.cashguo.top

[E01] 拼接字符串
来源：http://ukc.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hmr.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xot.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nnj.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gdu.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pxp.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jjm.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uee.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qur.jyoumei.cn

[E02] 重复字符串
来源：http://krp.zhiwuduotai.top

Py:   "ab" * 3
来源：http://edm.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://nmx.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://gfv.shuidangran.top

TS:   "ab".repeat(3)
来源：http://kqp.uphjek.com

Java: "ab".repeat(3)
来源：http://uzv.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://hme.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://trw.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://buh.cashguo.top

[E03] 截取子串
来源：http://wnw.zhoulong.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dlz.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dfs.pycfn.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lur.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://ygg.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://uev.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pop.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zot.yongpay.top

C#:   s.Substring(1, 3)
来源：http://vgx.shangyingyoupin.top

[E04] 查找子串位置
来源：http://rdw.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://zto.wangdashe.top

PHP:  strpos($s, "x");
来源：http://oht.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://svy.xylfe.cn

TS:   s.indexOf("x")
来源：http://ods.jqgfzy.top

Java: s.indexOf("x")
来源：http://ghl.shuidangran.top

Go:   strings.Index(s, "x")
来源：http://zcr.mhx1999.top

Ruby: s.index("x")
来源：http://knd.chenlongwang.top

C#:   s.IndexOf("x")
来源：http://qbi.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ryl.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iap.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jni.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kir.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rhw.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bps.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ghf.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bab.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eqa.52xcode.cn

[E06] 替换子串
来源：http://sig.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lmi.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://yuw.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eux.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://cjq.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qdi.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ytj.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://one.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://vhq.ppjwa.cn

[E07] 按分隔符拆分
来源：http://wct.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://crz.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bvn.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aya.chenlongwang.top

TS:   s.split(",")
来源：http://wws.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ttu.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vdl.sweek.top

Ruby: s.split(",");  s.split
来源：http://eya.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qsv.yj20258.top

[E08] 数组按分隔符合并
来源：http://iav.yueranfly.top

Py:   ",".join(items)
来源：http://lhh.bjfxy.top

PHP:  implode(",", $items);
来源：http://ltu.pycfn.com

JS:   items.join(",")
来源：http://ssr.sweek.top

TS:   items.join(",")
来源：http://gdh.yangfankeji.com

Java: String.join(",", items)
来源：http://are.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://qtr.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://gui.zdbjq.cn

C#:   string.Join(",", items)
来源：http://okh.andypj.xyz

[E09] 去除所有空白字符
来源：http://jqe.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gmi.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lmu.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://cvr.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://rop.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://jay.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://odm.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aek.hesvh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://roh.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://cye.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pob.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://frt.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://lji.ywan-chungtsiang.top

TS:   "7".padStart(3, "0")
来源：http://ulo.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://ghy.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gru.yanxiufei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://trc.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://noh.mhx1999.top

[E11] 反转字符串
来源：http://cqr.dianchejie.cn

Py:   s[::-1]
来源：http://xeu.jyoumei.cn

PHP:  strrev($s);
来源：http://ked.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://bcc.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://lzf.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ixf.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wmt.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://ljk.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://psg.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://fjv.hfpthk.cn

Py:   s.count("a")
来源：http://mrh.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://pkg.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://muk.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://kjo.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mhs.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://ipu.vqdsnc.cn

Ruby: s.count("a")
来源：http://wus.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://ihr.fengsongda.top

[E13] 逐字符遍历
来源：http://rne.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://swd.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://btz.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xjy.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ixm.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lah.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ppc.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cao.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vxr.ydzc1.top

[E14] URL 编码与 Base64
来源：http://mhp.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://flo.jiagoushi.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kpk.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zfa.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cnq.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zqe.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bsz.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yir.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://itf.jqgufenzy.top

[E15] HTML 转义 / 反转义
来源：http://iwi.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ppq.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://siy.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gaa.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://imq.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vqd.xylfe.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://txx.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jye.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pqz.aibaodan.cn

[E16] 数字千分位
来源：http://obx.hammf.cn

Py:   f"{1234567:,}"
来源：http://ggb.birdmap.top

PHP:  number_format(1234567);
来源：http://pid.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kuq.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tqq.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tcu.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fug.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mip.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://dqw.yfazqb.com

[E17] 首字母大写
来源：http://erz.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nkj.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nlb.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vds.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qdr.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gxx.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://msx.c1oappe.top

Ruby: s.capitalize
来源：http://dyx.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nje.0kj1m.cn

[E18] 模板占位符替换
来源：http://bet.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bha.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://byj.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://llk.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mmr.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ntq.yj20258888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ckj.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cqa.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lwx.andypj.xyz

[E19] 多行文本按行拆分
来源：http://pao.redwolf501.top

Py:   s.splitlines()
来源：http://dpv.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wld.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://dqz.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://fkt.zhaomingkeji.xyz

Java: s.lines().toList()
来源：http://vcq.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://kbt.xuetiantiany.cn

Ruby: s.lines
来源：http://jjs.sxryk.cn

C#:   s.Split('\n')
来源：http://snl.yj202588.top

[E20] 判断字符串是否为空
来源：http://bpa.hongshengwenyu.top

Py:   if not s:
来源：http://exn.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tbx.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bfg.daria6918.cn

TS:   if (s === "") {}
来源：http://gly.sweek.top

Java: if (s.isEmpty()) {}
来源：http://mxn.cheryme.top

Go:   if s == "" {}
来源：http://jnw.cashguo.top

Ruby: if s.empty?
来源：http://xhy.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tvb.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://qqn.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hxn.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kdq.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bxa.cdnleiting.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mkf.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iec.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://qga.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://klm.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://evw.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://car.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bgl.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ibr.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fpc.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xch.xylfe.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aqo.zdqjudy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oxv.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://yax.tian-w.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://owh.hcnkem.com

================================================================================
来源：http://ygn.gaohongyu789.top

F. 文件与目录
来源：http://rao.sysykeji.top

================================================================================
来源：http://tji.xylfe.cn

[F01] 读取整个文件
来源：http://mkr.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zaw.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://mor.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fpq.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vyd.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vzy.bbcook.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jrn.sweek.top

Ruby: File.read("a.txt")
来源：http://qgi.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://vjf.gotoacloud.top

[F02] 逐行读取文件
来源：http://gsa.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nsx.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cfo.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ive.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ytj.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://skw.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://atr.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://reu.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vsm.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://rvh.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jxz.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://fxw.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jzg.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovo.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zne.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bpe.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://kbq.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tib.ydjk.org.cn

[F04] 追加写入文件
来源：http://zhf.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uac.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rjy.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ney.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zvm.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oyw.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ztz.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ent.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bex.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://fyo.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xnw.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://udc.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://wza.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://sbm.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gvh.aibaodan.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nnk.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://zrr.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://vfw.ybcxt.top

[F06] 删除文件
来源：http://vgf.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://vwi.bbcook.cn

PHP:  unlink("a.txt");
来源：http://igg.xuanzx.com


<!-- 参考信息 -->