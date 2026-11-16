代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nvq.zdqjudy.top

Go:   // 手写双层循环
来源：http://nmh.zycfv.cn

Ruby: nested.flatten
来源：http://frj.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pge.xylfe.cn

[D19] 按字段分组
来源：http://mvi.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://atm.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ytw.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wzf.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cgo.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tay.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://ake.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://itu.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://omg.tian-w.cn

[D20] 统计每个元素出现次数
来源：http://vmc.sufxvd.cn

Py:   Counter(arr)
来源：http://wiw.hammf.cn

PHP:  array_count_values($arr);
来源：http://kbq.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bbe.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kms.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gxl.zycfv.cn

Go:   // 手写 map[T]int
来源：http://pvc.cucudq.cn

Ruby: arr.tally
来源：http://eep.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cev.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://wsv.zhoulong.xyz

Py:   x in arr
来源：http://zxz.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://nas.quarkkingdee.top

JS:   arr.includes(x)
来源：http://eee.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://exl.sjlbkw.cn

Java: list.contains(x)
来源：http://fto.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://ezg.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://yyp.cheryme.top

C#:   list.Contains(x)
来源：http://sod.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://aed.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xax.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fcs.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dvn.jiagoushi.top

TS:   [...arr];
来源：http://zeb.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://wzc.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gne.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://xax.daxiang520.top

C#:   new List<int>(list);
来源：http://oib.ppjwa.cn

[D23] reduce 累积计算
来源：http://jpr.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qpg.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://del.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ujn.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jqa.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vhw.zdbjq.cn

Go:   // 手写循环
来源：http://aww.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lgj.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tir.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://nbw.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uad.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kwk.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aun.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ctz.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dzp.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rav.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tqc.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qeb.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://ibr.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cde.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gch.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uuk.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://upr.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vld.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yoi.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nsp.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fhs.jinqigufen.top

[D26] 数组转字符串
来源：http://cxt.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://umd.hcnkem.com

PHP:  implode(", ", $arr);
来源：http://otk.sxryk.cn

JS:   arr.join(", ")
来源：http://upz.cdnleiting.top

TS:   arr.join(", ")
来源：http://ble.hammf.cn

Java: String.join(", ", list)
来源：http://ein.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://smv.pycfn.com

Ruby: arr.join(", ")
来源：http://khf.yvedp.cn

C#:   string.Join(", ", list)
来源：http://prz.zycfv.cn

================================================================================
来源：http://kgt.jianghu66.top

E. 字符串处理
来源：http://vkk.shuidangran.top

================================================================================
来源：http://vqf.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://vkc.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hit.jyoumei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tok.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://for.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vzl.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nsp.yvedp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rzj.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iax.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gkc.yueranfly.top

[E02] 重复字符串
来源：http://gpg.yangfankeji.com

Py:   "ab" * 3
来源：http://gej.quarkkingdee.top

PHP:  str_repeat("ab", 3);
来源：http://fay.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://jor.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://ijr.zhengqikj.top

Java: "ab".repeat(3)
来源：http://qxy.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://wbp.zycfv.cn

Ruby: "ab" * 3
来源：http://ofg.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://viv.bjfxy.top

[E03] 截取子串
来源：http://ihb.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://htw.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lqi.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zho.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://ejg.dashuyun.cn

Java: s.substring(1, 4)
来源：http://yqk.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vbe.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bmm.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://fbs.shzxlz.cn

[E04] 查找子串位置
来源：http://xba.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://bso.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://apl.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yfr.haohaochexian.top

TS:   s.indexOf("x")
来源：http://ctd.snrcjt.cn

Java: s.indexOf("x")
来源：http://uni.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://jrc.yangfankeji.com

Ruby: s.index("x")
来源：http://cln.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://rfe.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ois.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rec.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cwe.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dpw.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bjl.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lhu.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ica.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hrp.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mdq.hcnkem.com

[E06] 替换子串
来源：http://dsl.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uem.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://lzj.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lbk.cqqwz.cn

TS:   s.replaceAll("a", "b")
来源：http://ool.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kzi.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rjk.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kxu.shangyingyoupin.top

C#:   s.Replace("a", "b")
来源：http://mkk.nwbrower.top

[E07] 按分隔符拆分
来源：http://vri.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ble.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tsp.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kht.jianghu66.top

TS:   s.split(",")
来源：http://rmh.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://llj.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://maw.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://cun.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fhf.pengpengdd.cyou

[E08] 数组按分隔符合并
来源：http://dcb.yueranfly.top

Py:   ",".join(items)
来源：http://zmx.52xcode.cn

PHP:  implode(",", $items);
来源：http://kpw.wangdashe.top

JS:   items.join(",")
来源：http://sri.smart0.xyz

TS:   items.join(",")
来源：http://zxh.zhixingplan.top

Java: String.join(",", items)
来源：http://dvv.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://onj.nanxinkj.top

Ruby: items.join(",")
来源：http://kbc.sufxvd.cn

C#:   string.Join(",", items)
来源：http://isa.yuxming.cn

[E09] 去除所有空白字符
来源：http://ara.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rzo.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lkp.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://idv.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://pea.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://isd.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://meg.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://tsh.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ggz.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://jvk.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lbp.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yir.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://pwj.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://ywv.sysykeji.top

Java: String.format("%03d", 7)
来源：http://dlz.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://alw.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qew.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kut.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://zbk.mhx1999.top

Py:   s[::-1]
来源：http://egy.chenjidiqi.icu

PHP:  strrev($s);
来源：http://qgi.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://ehq.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://tkp.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wym.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zzj.redwolf501.top

Ruby: s.reverse
来源：http://nwm.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://qgk.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://gis.c1oappe.top

Py:   s.count("a")
来源：http://ope.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://ohn.havefunace.top

JS:   s.split("a").length - 1
来源：http://fwr.epnwcf.com

TS:   s.split("a").length - 1
来源：http://ytw.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yfx.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://egw.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://xxw.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://tzd.jiagoushi.top

[E13] 逐字符遍历
来源：http://sgn.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://iua.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nhc.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://suy.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://veg.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fzj.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ksf.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jnk.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qzq.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://hfk.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dbw.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cak.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://svb.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qdi.chenjidiqi.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cqe.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vsb.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tcj.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://swn.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://pdv.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kfp.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dwy.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yne.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xjj.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xge.dashuyun.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://klj.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hyd.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kac.tarul.cn

[E16] 数字千分位
来源：http://zxy.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://wwm.andypj.xyz

PHP:  number_format(1234567);
来源：http://rde.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xji.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://mvc.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rni.cashguo.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pcl.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pma.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://yad.zhengqikj.top

[E17] 首字母大写
来源：http://mpx.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qtn.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qev.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zzo.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lbk.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hji.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ovx.cashguo.top

Ruby: s.capitalize
来源：http://itc.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yes.nanxinkj.top

[E18] 模板占位符替换
来源：http://xai.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qqb.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://akl.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zyu.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bwx.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lkw.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qqf.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nrz.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fna.smart0.xyz

[E19] 多行文本按行拆分
来源：http://wqu.gotoacloud.top

Py:   s.splitlines()
来源：http://qtw.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xxf.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://ked.hywenlv.cn

TS:   s.split(/\r?\n/)
来源：http://eye.jlsjyb.cn

Java: s.lines().toList()
来源：http://ute.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://wkb.ctjpmb.com

Ruby: s.lines
来源：http://udg.tianlin.xyz

C#:   s.Split('\n')
来源：http://xip.c1oappe.top

[E20] 判断字符串是否为空
来源：http://jzj.fanxiaobao.xyz

Py:   if not s:
来源：http://axq.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://itp.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mqj.jyoumei.cn

TS:   if (s === "") {}
来源：http://djf.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://myk.cucudq.cn

Go:   if s == "" {}
来源：http://aix.sxryk.cn

Ruby: if s.empty?
来源：http://yic.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qsl.dashuyun.cn

[E21] 超长截断加省略号
来源：http://wtf.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qoj.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cgx.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mby.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pup.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bbc.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://pld.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bgm.xylfe.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jot.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://evw.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://izw.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xgu.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hhu.epnwcf.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vzf.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dui.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vwy.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://vsy.yfazqb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eky.hcnkem.com

================================================================================
来源：http://tlu.guannengcc.top

F. 文件与目录
来源：http://hdd.gzhubu.top

================================================================================
来源：http://cze.hongshengwenyu.top

[F01] 读取整个文件
来源：http://ytc.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://itr.pengpengdd.cyou

PHP:  file_get_contents("a.txt");
来源：http://ovf.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zpc.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://coo.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iyi.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dyc.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://iuo.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://mhh.ybcxt.top

[F02] 逐行读取文件
来源：http://nnk.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zep.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tjf.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rjk.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gxk.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://twi.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://txy.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bwx.jinqigufen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vwq.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://yoz.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eza.kuanghao11.cn


<!-- 参考信息 -->