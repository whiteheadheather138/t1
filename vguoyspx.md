代发 wailian999

[D19] 按字段分组
来源：http://vbo.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://usl.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kvk.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://egl.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://amg.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://biv.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://ckw.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://lfu.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xin.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://gdw.fengsongda.top

Py:   Counter(arr)
来源：http://dzu.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://tvt.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cly.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hre.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xdu.sysykeji.top

Go:   // 手写 map[T]int
来源：http://syb.ydjk.org.cn

Ruby: arr.tally
来源：http://idw.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hfx.xinyue.icu

[D21] 判断是否包含某元素
来源：http://ifa.havefunace.top

Py:   x in arr
来源：http://lfj.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://psx.yj20258888.top

JS:   arr.includes(x)
来源：http://ima.guannengcc.top

TS:   arr.includes(x)
来源：http://yol.cucudq.cn

Java: list.contains(x)
来源：http://gqc.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://frr.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://ilg.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://lte.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://ixp.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ztr.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://idm.snrcjt.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vlq.zhiwuduotai.top

TS:   [...arr];
来源：http://rkz.yj20258888.top

Java: new ArrayList<>(list);
来源：http://map.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kac.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://nnr.hcnkem.com

C#:   new List<int>(list);
来源：http://lfw.hesvh.cn

[D23] reduce 累积计算
来源：http://jqw.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://obd.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mjg.daria6918.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gns.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jou.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://hll.ydzc1.top

Go:   // 手写循环
来源：http://ess.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mgt.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aap.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://mhi.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://obr.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zmv.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fdn.gaohongyu789.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dob.gogol.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gej.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vev.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gtv.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rmr.sweek.top

[D25] Set 集合去重与交并差
来源：http://atu.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fkl.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://esj.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dve.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pqd.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://law.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mnq.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://suh.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jyq.yanxiufei.cn

[D26] 数组转字符串
来源：http://gdp.jinqigfzy.top

Py:   ", ".join(map(str, arr))
来源：http://ojw.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://vrc.dashuyun.cn

JS:   arr.join(", ")
来源：http://jra.316326.xyz

TS:   arr.join(", ")
来源：http://dce.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://kbj.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://rui.sysykeji.top

Ruby: arr.join(", ")
来源：http://shx.jianghu66.top

C#:   string.Join(", ", list)
来源：http://cpe.redwolf501.top

================================================================================
来源：http://whn.jinyuanbaomall.cn

E. 字符串处理
来源：http://fzr.yj202588.top

================================================================================
来源：http://cus.smart0.xyz

[E01] 拼接字符串
来源：http://oxx.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zjt.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nhm.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iep.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxr.fehbvm.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rsi.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://onq.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nme.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hev.hesvh.cn

[E02] 重复字符串
来源：http://syx.ppjwa.cn

Py:   "ab" * 3
来源：http://pvt.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://tyo.meibo888.top

JS:   "ab".repeat(3)
来源：http://mur.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://mpi.sxryk.cn

Java: "ab".repeat(3)
来源：http://drm.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://vfc.cqqwz.cn

Ruby: "ab" * 3
来源：http://xcg.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xfo.cheryme.top

[E03] 截取子串
来源：http://gsk.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ofw.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iir.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zmc.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://oin.yvedp.cn

Java: s.substring(1, 4)
来源：http://pfz.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lym.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bdv.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://jai.cheryme.top

[E04] 查找子串位置
来源：http://lur.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://qww.ybcxt.top

PHP:  strpos($s, "x");
来源：http://uvl.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://adu.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://tze.dashuyun.cn

Java: s.indexOf("x")
来源：http://rfh.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://pdh.jianghu66.top

Ruby: s.index("x")
来源：http://poh.yvedp.cn

C#:   s.IndexOf("x")
来源：http://fkk.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mcm.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sjx.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gew.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fjz.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cnv.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ndi.jlsjyb.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eud.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://acz.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cob.0kj1m.cn

[E06] 替换子串
来源：http://bgk.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wto.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://dws.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gti.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://wjf.nwbrower.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://npr.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ffw.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rkw.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://vxr.yongpay.top

[E07] 按分隔符拆分
来源：http://ziv.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://htt.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gmq.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lxl.tanke756.top

TS:   s.split(",")
来源：http://yjh.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://pif.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xim.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://gvk.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tse.xziqi.cn

[E08] 数组按分隔符合并
来源：http://okh.xziqi.cn

Py:   ",".join(items)
来源：http://jvm.sysykeji.top

PHP:  implode(",", $items);
来源：http://plk.316326.xyz

JS:   items.join(",")
来源：http://vtn.vqdsnc.cn

TS:   items.join(",")
来源：http://cut.sweek.top

Java: String.join(",", items)
来源：http://lsu.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://eku.xziqi.cn

Ruby: items.join(",")
来源：http://lzr.tian-w.cn

C#:   string.Join(",", items)
来源：http://vkw.ybcxt.top

[E09] 去除所有空白字符
来源：http://sya.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ssq.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kee.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://fek.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ypw.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://dnw.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://asy.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://ufq.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kta.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://qfg.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xni.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ill.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://kcg.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://vnh.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://bme.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ula.bjfxy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qor.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sra.sxryk.cn

[E11] 反转字符串
来源：http://lnz.ydjk.org.cn

Py:   s[::-1]
来源：http://qgp.zdqjudy.top

PHP:  strrev($s);
来源：http://erp.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://emt.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://mze.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vxx.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dis.yueranfly.top

Ruby: s.reverse
来源：http://col.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://uta.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://ydz.yfazqb.com

Py:   s.count("a")
来源：http://aoh.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://fuz.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://xyz.52xcode.cn

TS:   s.split("a").length - 1
来源：http://unz.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://loz.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://aza.chenlongwang.top

Ruby: s.count("a")
来源：http://dfa.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://nbt.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://thi.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://ift.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://idh.wangdashe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gja.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vxa.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ecg.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jpe.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cqf.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iga.yuxming.cn

[E14] URL 编码与 Base64
来源：http://awk.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vlx.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vop.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qtv.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ouv.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://scn.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ozw.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rpu.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mma.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://nku.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nrr.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zll.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://exw.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://spy.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zzp.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dsk.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oey.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://voo.xuanzx.com

[E16] 数字千分位
来源：http://wuj.yvedp.cn

Py:   f"{1234567:,}"
来源：http://xxi.andypj.xyz

PHP:  number_format(1234567);
来源：http://qwv.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kho.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xyt.pycfn.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lra.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ytf.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rlf.ivvv.top

C#:   1234567.ToString("N0")
来源：http://ohk.shzxlz.cn

[E17] 首字母大写
来源：http://qfa.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ifu.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rmv.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://agc.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vpf.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qhj.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pwp.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://jnc.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uik.daxiang520.top

[E18] 模板占位符替换
来源：http://scd.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jwu.9152youxi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kxu.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xuo.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://egx.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ypr.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fpd.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uxi.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ipi.ywan-chungtsiang.top

[E19] 多行文本按行拆分
来源：http://iku.hongshengwenyu.top

Py:   s.splitlines()
来源：http://yql.sweek.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://onw.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://qou.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://geq.daria6918.cn

Java: s.lines().toList()
来源：http://whc.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://ayy.xinyue.icu

Ruby: s.lines
来源：http://cgb.bjfxy.top

C#:   s.Split('\n')
来源：http://pfr.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://asr.daxiang520.top

Py:   if not s:
来源：http://jfe.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oss.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bwn.hysaishi.cn

TS:   if (s === "") {}
来源：http://ipa.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://jej.jianghu66.top

Go:   if s == "" {}
来源：http://oer.feifeiyinyue.top

Ruby: if s.empty?
来源：http://bzy.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xcp.sweek.top

[E21] 超长截断加省略号
来源：http://fyo.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cep.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oik.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tsz.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://izg.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cax.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://yaq.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://leu.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gij.hammf.cn

[E22] 字节长度与字符长度
来源：http://psz.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ceu.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nuo.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vzm.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jgh.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kjn.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dtb.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://ziq.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kbq.xuetiantiany.cn

================================================================================
来源：http://ujm.zhengqikj.top

F. 文件与目录
来源：http://xwl.hcnkem.com

================================================================================
来源：http://don.sysykeji.top

[F01] 读取整个文件
来源：http://mxa.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xrt.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://uqp.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uym.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ldl.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qkq.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mre.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://tir.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://tct.hesvh.cn

[F02] 逐行读取文件
来源：http://hhx.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vlf.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wid.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dlr.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fzj.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yha.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zid.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vwe.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wuv.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://ycl.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://plc.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xck.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fwl.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lxz.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bni.yj202588.top


<!-- 参考信息 -->